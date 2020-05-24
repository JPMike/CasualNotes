### ps usage guide

ps, process status

format: ps [options]

#### options:
- `-e`: show all processes
- `-a`: show current terminal processes
- `-u`: show user info of process
- `-f`: show process relation

#### output fields:
- `USER`
- `PID`
- `START`: process activate time
- `%CPU`
- `%MEM`
- `VSZ`: usage of virtual memery, unit is K
- `RSS`
- `TTY`
- `STAT`
    - `D`: uninterruptible sleep
    - `R`
    - `S`: sleep
    - `T`
    - `Z`: zombie
    - `X`
    - `<`: high priority
    - `N`: low priority
    - `s`: has child process
    - `l`: multiple thread, clone thread
- `TIME`: usage of total CPU time
- `COMMAND`
- `NI`
- `PRI`
- `PPID`
- `WCHAN`: name of kernel event which process wait for

#### common use case
- `ps -ef`
- `ps -u root`
- `ps -ef | grep java`
- `ps aux`
- `ps -efl`
- `ps -ejH`: to print a process tree
- `ps -o %cpu,stat --pid 1234`
- `ps aux | more`