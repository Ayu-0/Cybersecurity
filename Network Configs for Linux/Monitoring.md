# Network Monitoring Tools :

## 1. Check open ports (netstat) :


## 2. Monitoring Network Traffic () :



## 3. Detect rootkits and suspicious activity (rkhunter) :

**What is rootkit?**
-  malware program that enables cyber criminals to gain access to and infiltrate data from machines without being detected. 

**Types of rootkits?**
1. Firmware rootkits
2. Bootloader rootkits
3. Memory rootkits
4. Applications rootkits
5. Kernel mode rootkits

**Check for rootkits**

- We'll use rkhunter to detect rootkits
- So what does rkhunter check?
It checks for:

SHA256 hash changes
Files commonly created by rootkits
Executables with anomalous file permissions
Suspicious strings in kernel modules, and
Hidden files in system directories

**How to scan?**
run simple check cmmd -
```
sudo rkhunter -c
```
**Run this cmmd for more usage ``` sudo rkhunter -h```**

**How to remove detected rootkits?**
- There is no direct removal
- So, we do have to remove manually
- terminate the process and remoe them permanently

