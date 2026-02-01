1. Process Management

1) ps aux – list all running processes
2) top – real-time CPU and memory usage
3) htop – enhanced interactive process viewer/ human redable formate 
4) kill <PID> – terminate a process by PID
5) kill -9 <PID> – force kill a stuck process
6) pkill <name> – kill process by name
7) nice – start process with priority
8) renice – change priority of running process

2. File System & Navigation

1) pwd – show current directory
2) ls -l – list files with details
3) cd <dir> – change directory
4) cd .. – move one level back
5) mkdir <dir> – create directory
6) rm -rf <dir> – delete directory recursively
7) cp <src> <dest> – copy files
8) mv <src> <dest> – move/rename files
9) touch <file> – create empty file
10) cat <file> – view file contents

3. Disk & Memory Usage

1) df -h – disk usage by filesystem
2) du -sh <dir> – disk usage of directory
3) free -m – how much memory usage free in MB
4) lsblk – list block devices

4. Networking & Troubleshooting

1) ip addr – show network interfaces and IPs
2) ping <host> – test network connectivity
3) curl <url> – test HTTP/HTTPS endpoints
4) ss -tuln – show listening ports
5) netstat -rn – view routing table
6) dig <domain> – DNS lookup; check name resolution and DNS records
7) nslookup <domain> – quick DNS lookup to verify domain → IP mapping

5. System & Logs

1) uname -r – show running kernel version
2) uptime – system running time and load
3) journalctl -xe – view systemd logs
4) systemctl status <service> – check service status



