### Linux IO

#### Example C code

```bash
int main()
{
    char c;
    int in;

    in = open("in.txt", 0_RDONLY);
    read(in, &c, 1);
    close(in);
    return 0;
}
```

#### Linux IO stack

[Linux IO stack](http://www.ilinuxkernel.com/files/Linux.IO.stack_v1.0.pdf)

[Generic Block Layer](https://www.ilinuxkernel.com/files/Linux.Generic.Block.Layer.pdf)


##### IO Scheduler Layer

- check algorithmn

    ```bash
    dmesg | grep -i scheduler
    ```

