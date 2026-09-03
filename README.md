# Configure-Authentication-and-Authorization-in-Linux

# Linux Authentication and Authorization Lab

## Overview
This lab introduces Linux authentication and authorization by creating users and groups, assigning passwords, and managing file and directory permissions using both symbolic and absolute (octal) modes. :contentReference[oaicite:0]{index=0}

## Objectives
- Create and manage Linux groups
- Add and manage user accounts
- Assign users to groups
- Configure authentication with passwords
- Modify file and directory permissions
- Use symbolic and octal permission modes
- Verify user access and authorization :contentReference[oaicite:1]{index=1}

## Technologies Used
- Linux (Ubuntu/CSE-LABVM)
- VirtualBox
- Linux Terminal
- Linux User & Group Management
- File Permission Management

## Key Linux Commands
```bash
sudo su
groupadd HR
adduser jenny
adduser joe
usermod -G HR jenny
usermod -G HR joe
cat /etc/group
cat /etc/passwd
cat /etc/shadow
pwd
cd
ls -l
chmod
touch
su
exit
```

## Skills Learned
- Linux user and group administration
- Authentication and authorization concepts
- Password management
- File system navigation
- Symbolic (`chmod o-x`) permissions
- Absolute (`chmod 705`) permissions
- Access control and least privilege
- Reading Linux system files (`/etc/passwd`, `/etc/group`, `/etc/shadow`)

## Permission Values
| Number | Permission |
|---------|------------|
| 7 | rwx |
| 6 | rw- |
| 5 | r-x |
| 4 | r-- |
| 3 | -wx |
| 2 | -w- |
| 1 | --x |
| 0 | --- |

## Key Takeaways
- Authentication verifies a user's identity, while authorization determines what resources they can access.
- Groups simplify permission management across multiple users.
- Linux permissions control read, write, and execute access for the owner, group, and others.
- The `chmod` command supports both symbolic and octal permission formats.
- Proper permission management is essential for Linux system security and follows the Principle of Least Privilege.

---
**Source:** Cisco Networking Academy – *Lab: Configure Authentication and Authorization in Linux*. :contentReference[oaicite:2]{index=2}
