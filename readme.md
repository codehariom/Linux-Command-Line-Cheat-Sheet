# **Ultimate Linux Command Line Cheat Sheet**  

This cheat sheet provides a **comprehensive** list of **essential Linux commands** for system administration, file management, networking, and more.  

---

## **📌 1. System Information**  
| Command | Description |
|---------|-------------|
| `uname -a` | Show **all system information** (kernel, hostname, etc.) |
| `uname -r` | Display **kernel version** |
| `lsb_release -a` | Show **Linux distribution details** |
| `uptime` | Display **system uptime & load average** |
| `hostname` | Show **hostname** |
| `hostname -I` | List **all IP addresses** |
| `last reboot` | Show **reboot history** |
| `date` | Display **current date & time** |
| `cal` | Show **calendar** |
| `w` | List **logged-in users & their processes** |
| `whoami` | Show **current username** |

---

## **🖥️ 2. Hardware Information**  
| Command | Description |
|---------|-------------|
| `cat /proc/cpuinfo` | Show **CPU details** |
| `cat /proc/meminfo` | Display **memory information** |
| `free -h` | Show **RAM usage** (human-readable) |
| `lspci -tv` | List **PCI devices** (GPU, network cards, etc.) |
| `lsusb -tv` | List **USB devices** |
| `dmidecode` | Show **BIOS & hardware details** |
| `hdparm -i /dev/sda` | Check **disk info** |
| `hdparm -tT /dev/sda` | Test **disk read speed** |

---

## **📊 3. Performance Monitoring**  
| Command | Description |
|---------|-------------|
| `top` | Interactive **process monitor** |
| `htop` | Enhanced **process viewer** |
| `mpstat 1` | Show **CPU stats** (per core) |
| `vmstat 1` | Display **virtual memory stats** |
| `iostat 1` | Monitor **disk I/O stats** |
| `tcpdump -i eth0` | Capture **network traffic** |
| `netstat -tuln` | List **open ports & services** |

---

## **👥 4. User Management**  
| Command | Description |
|---------|-------------|
| `id` | Show **user & group IDs** |
| `last` | View **login history** |
| `who` | List **logged-in users** |
| `useradd -m username` | **Create a new user** |
| `userdel username` | **Delete a user** |
| `usermod -aG groupname username` | **Add user to a group** |
| `passwd username` | **Change user password** |

---

## **📂 5. File & Directory Commands**  
| Command | Description |
|---------|-------------|
| `ls -al` | List **all files (including hidden)** |
| `pwd` | Show **current directory** |
| `mkdir dirname` | **Create a directory** |
| `rm file` | **Delete a file** |
| `rm -rf dirname` | **Force-delete a directory** |
| `cp file1 file2` | **Copy a file** |
| `cp -r dir1 dir2` | **Copy a directory** |
| `mv file1 file2` | **Move/rename a file** |
| `ln -s /path linkname` | **Create a symlink** |
| `touch file` | **Create an empty file** |
| `cat file` | **View file contents** |
| `less file` | **View file page-by-page** |
| `head -n 5 file` | Show **first 5 lines** |
| `tail -f file` | **Follow file changes** |

---

## **🔍 6. Searching & Data Manipulation**  
| Command | Description |
|---------|-------------|
| `grep "text" file` | **Search for text** in a file |
| `grep -r "text" /dir` | **Recursively search** |
| `find / -name "*.log"` | **Find files by name** |
| `locate filename` | **Quick file search** (updatedb) |
| `awk '{print $1}' file` | **Extract column** from text |
| `sed 's/old/new/g' file` | **Replace text** in a file |
| `sort file` | **Sort file contents** |
| `diff file1 file2` | **Compare two files** |

---

## **⚙️ 7. Process Management**  
| Command | Description |
|---------|-------------|
| `ps aux` | List **all running processes** |
| `kill -9 PID` | **Force-kill a process** |
| `killall processname` | **Kill all matching processes** |
| `bg` | Send to **background** |
| `fg` | Bring to **foreground** |
| `nohup command &` | Run **after logout** |

---

## **🔒 8. File Permissions**  
| Permission | Meaning | Example |
|-----------|---------|---------|
| `chmod 755 file` | `rwxr-xr-x` (User: rwx, Group: r-x, Others: r-x) |
| `chmod 644 file` | `rw-r--r--` (User: rw-, Group: r--, Others: r--) |
| `chown user:group file` | **Change owner & group** |

---

## **🌐 9. Networking**  
| Command | Description |
|---------|-------------|
| `ifconfig` | Show **network interfaces** |
| `ping google.com` | **Test connectivity** |
| `dig google.com` | **DNS lookup** |
| `netstat -tuln` | List **open ports** |
| `ssh user@host` | **Connect via SSH** |
| `scp file user@host:/path` | **Secure file copy** |
| `wget URL` | **Download a file** |
| `curl URL` | **Fetch URL content** |

---

## **📦 10. Archives & Compression**  
| Command | Description |
|---------|-------------|
| `tar -cvf archive.tar dir/` | **Create a tar archive** |
| `tar -xvf archive.tar` | **Extract tar archive** |
| `tar -czvf archive.tar.gz dir/` | **Compress with gzip** |
| `tar -xzvf archive.tar.gz` | **Extract gzip archive** |
| `zip archive.zip file` | **Create ZIP file** |
| `unzip archive.zip` | **Extract ZIP file** |

---

## **📌 11. Package Management**  
| Command | Description |
|---------|-------------|
| `apt update` | **Update package list** (Debian/Ubuntu) |
| `apt install package` | **Install a package** |
| `apt remove package` | **Remove a package** |
| `yum install package` | **Install (RHEL/CentOS)** |
| `dnf install package` | **Install (Fedora)** |
| `rpm -i package.rpm` | **Install RPM package** |

---

## **💾 12. Disk Usage**  
| Command | Description |
|---------|-------------|
| `df -h` | Show **disk space usage** |
| `du -sh dir/` | **Directory size** |
| `fdisk -l` | List **partitions** |
| `mount /dev/sda1 /mnt` | **Mount a filesystem** |

---

## **🚀 Bonus: Shortcuts & Tips**  
- `Ctrl + C` → **Kill current process**  
- `Ctrl + Z` → **Suspend process**  
- `Ctrl + D` → **Exit terminal**  
- `!!` → **Rerun last command**  
- `history` → **View command history**  

---

### **📚 Conclusion**  
This cheat sheet covers **90% of daily Linux commands**. Bookmark it for quick reference!  

🔹 **For more details:** Use `man command` (e.g., `man ls`) for full documentation.  

## Folow for more [LinkedIn](https://www.linkedin.com/in/realhariom/) and [Github](github.com/codehariom/)

### 🚀 Happy Coding Journey