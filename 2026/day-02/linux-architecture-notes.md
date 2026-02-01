1. Core Components of Linux

Kernel - The core of the OS; runs in privileged (kernel) mode
Manages: CPU scheduling, Memory (RAM, virtual memory), Devices & drivers, Filesystems
Directly connect to hardware

User Space - Where users and applications run
Includes: Shells (bash, sh), System libraries (glibc), User commands (ls, ps, systemctl)
Applications request kernel services via system calls

Init System (systemd) - First process started by the kernel (PID 1)
Responsible for bringing the system to a usable state

2. How Processes Are Created & Managed

A process is a running instance of a program
Creation flow: fork() → creates a child process, exec() → loads a new program into the process
Each process has: PID (Process ID), Parent PID, State
Common Process States -
1) Running (R) – executing on CPU
2) Sleeping (S) – waiting for I/O or event
3) Uninterruptible Sleep (D) – waiting on disk/network I/O
4) Stopped (T) – paused (usually by signal)
5) Zombie (Z) – finished execution, waiting for parent to collect status

3. What systemd Does (and Why It Matters)

Starts and manages services, daemons, mounts, timers
Replaces older init systems (SysVinit)
Key benefits: Parallel service startup (faster boot), Automatic restarts of failed services, Centralized logging with journalctl
systemd Concepts: 
1) Unit: configuration object (service, socket, timer)
2) Target: group of units (similar to runlevels)

4. Commands Used Daily (DevOps)

1) ps – view running processes
2) top / htop – real-time process monitoring
3) systemctl – manage services
4) journalctl – view system logs
5) df / du – disk usage analysis
6) pwd – show current working directory
7) cd – change directory
8) cd .. – move one directory up
9) ls – list files and directories
10) mkdir – create a new directory
11) touch – create an empty file
12) cp – copy files or directories
13) mv – move or rename files/directories
14) rm – delete files or directories
15) cat – view file contents
16) uname -r – show running kernel version
17) ip addr – display network interfaces and IPs
18) ping – test network connectivity
19) free – show memory usage
20) df – show disk space usage









