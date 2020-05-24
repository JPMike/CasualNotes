### system status guide

#### show system up time
```bash
uptime
```

#### show login user
```bash
who -a
```

#### show system version info
```bash
uname -a
```

#### show current environment variable
```bash
export
```

#### show directory and file space usage
```bash
du -h --max-depth=1
# show only current directory
du -sh
```

#### show mount point space
```bash
df -h
```

#### show memory usage
```bash
free -h
```

#### show process memory usage
```bash
pmap <pid>
```

#### show virtual memory statistics info
```bash
vmstat
```

#### show ip address
```bash
ip <addr>
```

#### show process relation
```bash
pstree
```

#### watch
```bash
# memory info every 1 second
watch -n 1 cat /proc/meminfo
# network info
watch -n 1 cat /proc/net/dev
```