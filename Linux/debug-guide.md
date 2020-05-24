### debug guide

#### example program
```c
// cmd_test.c
#include<stdio.h>

int test(int a, int b)
{
    return a / b;
}

int main(int argc, char *argv[])
{
    int a = 10;
    int b = 0;
    printf("a=%d,b=%d\n", a, b);
    test(a, b);
    return 0;
}
```

#### get elf file
```bash
gcc -g -o cmd_test cmd_test.c
./cmd_test
```

#### common use case
```
# basic info
file cmd_test
readelf -h cmd_test
# dependence file
ldd cmd_test
# show function or global variables
nm cmd_test
# sort by address order
nm -n cmd_test
# print pritable strings
strings cmd_test
# check text segment volumn
size cmd_test
# remove symbol info of elf file
ls -al cmd_test
strip cmd_test
ls -al cmd_test
# disassemble
objdump -d cmd_test
objdump -d cmd_test --start-address=0x1234 --stop-address=0x5678
# check port usage
netstat -anp
# check core file setting
ulimit -c
ulimit -c unlimited
ulimit -c 10 # 10kb
```
