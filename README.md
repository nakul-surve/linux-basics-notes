# Linux Basics Notes

This repository contains Linux commands and notes that I am learning as part of my DevOps journey.

Topics:
- Basic Linux commands
- File and directory management
- Permissions
- Process basics

More updates coming soon 


# Basic Linux Commands

# File & Directory Commands
- pwd – show current directory
- ls – list files and directories
- cd – change directory
- mkdir – create directory
- rmdir – remove directory
- rm – remove files/directories

# File Viewing Commands
- cat – view file content
- less – view file page by page
- head – view first lines
- tail – view last lines

# Permissions (Basics)
- chmod – change permissions
- chown – change owner


## Process & System Commands

- ps – view running processes
- top – monitor system processes
- uptime – system running time
- whoami – current user


## Linux File Permissions

Linux controls access to files using permissions.

### Permission Types
- r (read): allows viewing file content
- w (write): allows modifying file content
- x (execute): allows running a file or script

### Permission Groups
- User (owner)
- Group
- Others

### Example
-rwxr-xr--

This means:
- User: read, write, execute
- Group: read, execute
- Others: read only

### Common Commands
- ls -l
- chmod
- chown

### Why It Matters in DevOps
- Securing servers
- Controlling access
- Preventing unauthorized execution


## Linux Process Management

Processes are running programs in Linux. Managing them is critical in servers and production systems.

### Common Commands
- ps        → shows running processes
- top       → real-time process monitoring
- htop      → improved version of top (if installed)
- kill      → terminate a process
- kill -9   → force kill a process

### Example
ps aux | grep nginx

This helps find running services like web servers.

### Why It Matters in DevOps
- Monitor application health
- Troubleshoot high CPU or memory usage
- Restart failed services

## Linux Logs Basics

Logs help understand what happened in a system.

### Common Log Locations
- /var/log/syslog
- /var/log/auth.log
- /var/log/nginx/

### Useful Commands
- cat
- less
- tail
- tail -f

### Example
tail -f /var/log/syslog

### Why Logs Matter
- Debugging issues
- Security monitoring
- Incident investigation

Learning focus: Linux fundamentals for cloud and production systems.
