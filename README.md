# 🐧 Linux Learning Platform

A beginner-friendly, GitHub-ready Linux learning resource. This repository organizes class notes into separate topic-wise lessons, explains what common commands do, and gives you a practical path to learn Linux step by step.

![Linux Learning Roadmap](images/linux-learning-roadmap.png)

## 🎯 What you'll learn

- Linux and operating-system fundamentals
- Terminal navigation and filesystem structure
- Creating, reading, and editing files
- Linux permissions, ownership, users, and groups
- Searching, sorting, and processing text
- Package management, logs, and scheduled tasks
- Networking, storage, processes, and system monitoring
- Secure file transfer and Linux security basics

## 🗂️ Repository structure

```text
linux-learning-platform/
├── README.md
├── images/
│   ├── linux-learning-roadmap.png
│   ├── linux-command-cheatsheet.png
│   └── linux-filesystem-hierarchy.jpeg
└── topics/
    ├── 01-linux-fundamentals.md
    ├── 02-filesystem-navigation.md
    ├── 03-file-creation-and-viewing.md
    ├── 04-vim-editor.md
    ├── 05-file-details.md
    ├── 06-permissions-and-ownership.md
    ├── 07-user-and-group-management.md
    ├── 08-links.md
    ├── 09-text-search-grep.md
    ├── 10-sort.md
    ├── 11-uniq.md
    ├── 12-cut-and-pipelines.md
    ├── 13-wc.md
    ├── 14-package-management.md
    ├── 15-archive-and-compression.md
    ├── 16-file-transfer.md
    ├── 17-networking.md
    ├── 18-logs-and-troubleshooting.md
    ├── 19-scheduling-with-cron.md
    ├── 20-linux-security.md
    └── 21-system-monitoring.md
```

## 📚 Topic-wise lessons

| # | Topic | What it covers |
|---|---|---|
| 01 | [Linux Fundamentals](topics/01-linux-fundamentals.md) | Linux, CLI, shell, starter commands |
| 02 | [Filesystem Navigation](topics/02-filesystem-navigation.md) | `pwd`, `ls`, `cd`, absolute and relative paths |
| 03 | [File Creation and Viewing](topics/03-file-creation-and-viewing.md) | `touch`, `mkdir`, `cat`, `echo`, `rm` |
| 04 | [Vim Text Editor](topics/04-vim-editor.md) | `vi`, `vim`, modes, save, search, edit |
| 05 | [Understanding File Details](topics/05-file-details.md) | `ls -l`, file type, owner, group, size, date |
| 06 | [Permissions and Ownership](topics/06-permissions-and-ownership.md) | `chmod`, `chown`, `chgrp`, ACL |
| 07 | [User and Group Management](topics/07-user-and-group-management.md) | User and group administration |
| 08 | [Hard Links and Symbolic Links](topics/08-links.md) | `ln`, `ln -s`, inode basics |
| 09 | [Searching Text with grep](topics/09-text-search-grep.md) | `grep`, `-i`, `-n`, `-v`, `-w` |
| 10 | [Sorting Text](topics/10-sort.md) | `sort`, numeric, reverse, field sorting |
| 11 | [Removing Duplicates](topics/11-uniq.md) | `uniq`, `uniq -c` |
| 12 | [Extracting Fields](topics/12-cut-and-pipelines.md) | `cut`, delimiters, pipes (`|`) |
| 13 | [Counting with wc](topics/13-wc.md) | Count lines, words, and bytes |
| 14 | [Package Management](topics/14-package-management.md) | `yum`, `rpm`, package install/update/remove |
| 15 | [Archiving and Compression](topics/15-archive-and-compression.md) | `tar`, `gzip`, `bzip2`, `xz` |
| 16 | [Secure File Transfer](topics/16-file-transfer.md) | `scp`, `rsync`, SSH |
| 17 | [Linux Networking](topics/17-networking.md) | IP addresses, IPv4, IPv6, CIDR |
| 18 | [Logs and Troubleshooting](topics/18-logs-and-troubleshooting.md) | `/var/log`, `last`, `lastb`, web logs |
| 19 | [Task Scheduling with cron](topics/19-scheduling-with-cron.md) | Schedule recurring tasks |
| 20 | [Linux Security](topics/20-linux-security.md) | Updates, least privilege, services, backups |
| 21 | [System Monitoring](topics/21-system-monitoring.md) | CPU, RAM, disk, processes, ports |

## 🧰 Linux command quick reference

![Linux Command Quick Reference](images/linux-command-cheatsheet.png)

| Command | Used for |
|---|---|
| `pwd` | Print the current working directory |
| `ls -lah` | List files, including hidden files, with readable sizes |
| `cd /path` | Change to a directory |
| `mkdir -p dir/subdir` | Create a directory path |
| `touch file.txt` | Create an empty file or update its timestamp |
| `cp source destination` | Copy files or directories |
| `mv source destination` | Move or rename files |
| `cat file.txt` | Print file contents |
| `less file.txt` | Read a file page by page |
| `head -n 10 file.txt` | Show the first 10 lines |
| `tail -n 10 file.txt` | Show the last 10 lines |
| `grep -n 'word' file.txt` | Search for a word and show matching line numbers |
| `find /path -name 'file*'` | Find files by name |
| `chmod 644 file.txt` | Set file permissions |
| `chown user:group file.txt` | Change owner and group |
| `df -h` | Show filesystem disk space |
| `du -sh folder/` | Show a folder's total size |
| `free -h` | Show memory usage |
| `top` | Monitor running processes |
| `ps -ef` | List running processes |
| `ip addr` | Show network interfaces and IP addresses |
| `ss -tulnp` | Show listening TCP/UDP sockets |
| `tar -czf backup.tar.gz folder/` | Create a compressed archive |
| `scp file user@host:/path/` | Copy a file to a remote host over SSH |

## 🖥️ Linux filesystem hierarchy

![Linux Filesystem Hierarchy](images/linux-filesystem-hierarchy.jpeg)

A few important directories:

- `/` — root of the filesystem
- `/home` — regular users' home directories
- `/root` — root user's home directory
- `/etc` — system and application configuration
- `/var/log` — log files
- `/tmp` — temporary files
- `/usr` — user-space programs and shared resources
- `/bin` and `/sbin` — essential command binaries (layout can vary across distributions)

## 🚀 How to use this repository

1. Start with topic 01 and follow the lessons in order.
2. Open a Linux virtual machine, cloud instance, or WSL environment to practise.
3. Read one topic, run the examples, and write down the output.
4. Use `man command` (example: `man ls`) to explore command options.
5. Practise safely in a test directory before running commands on important systems.

### Suggested practice setup

- Ubuntu or another Linux distribution
- A terminal or SSH client
- A non-root practice user
- A test folder for file and permission exercises

## ⚠️ Safety notes

- Avoid practising destructive commands such as `rm -rf` on important paths.
- Do not copy commands using `sudo` or root privileges unless you understand their effect.
- Package commands differ by distribution: `yum`/`dnf` are common on RHEL-family systems; `apt` is used on Debian/Ubuntu.
- Some commands in the original class notes are distribution-specific. Check your OS and use `man` pages for the correct syntax.

## 🤝 Contributions

Found an error or want to add a Linux topic? Open an issue or submit a pull request with a clear explanation and tested examples.

## 📌 Learning goal

Learn the command, understand the task it performs, practise it in a safe environment, and verify the result. Linux becomes much easier when you use it every day.

---

**Made for Linux learners | Learn • Practise • Build**
