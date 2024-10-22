**Text Linux System Information**
### 1 Display kernel and system architecture information
```bash
uname -a
```

### 2 Show CPU Information
```bash
cara /proc/cpuinfo
```

### 3 Display memory usage (RAM)
```bash
free -h
```

### 4 Get System uptime
```bash
uptime
```

### 5 Show Detailed sustem resource usage
```bash
top
```

### 6 Disk usage of all mounted filesystems
```bash
df -h
```

### 7 Chek current disk usage per direcetory
```bash
du -sh *
```

### 8 Show PCI devices information
```bash
lspci
```

### 9 Display usb devices information
```bash
lsusb
```

### 10 network interface information
```bash
ifconfig
```

### 11 Show kernel messages (useful for debugging hardware)
```bash
dmesg | less
```

### 12 Check system logs (for recent activity/erros)
```bash
tail -f /var/log/syslog
```

### 13 Display block device information (disks, partitions)
```bash
lsblk
```

### 14 list all loaded kernel modules
```bash
lsmod
```

### 15 show system hostname
```bash
hostname
```