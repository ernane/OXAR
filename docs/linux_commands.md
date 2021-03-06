# Linux Commands

The goal of this document is to list random linux commands that may help debug and/or troubleshoot errors.

Purpose | Command | Description
------ | ------ | ------
Find large files | `du -a / | sort -n -r | head -n 20` | Finds largest 20 files/directories
Firewall open ports | `firewall-cmd --list-all` | Uses `firewalld`
Prevent having to enter password each time you do a `sudo` call | `sudo bash -c "echo '<username> ALL = NOPASSWD : ALL' | (EDITOR='tee -a' visudo)"` |
[Open ports](http://www.cyberciti.biz/faq/how-do-i-find-out-what-ports-are-listeningopen-on-my-linuxfreebsd-server/) | `netstat --listen` |
[Delete User](http://www.cyberciti.biz/faq/linux-remove-user-command/) | `userdel username` | Add option `-r` to remove the user's home directory
[Set DNS Servers](http://www.cyberciti.biz/faq/howto-linux-bsd-unix-set-dns-nameserver/) | `vi /etc/resolve.conf` then add `nameserver <ip>` |
