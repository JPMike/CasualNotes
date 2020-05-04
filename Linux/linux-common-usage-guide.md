### linux common usage guide

- list directory contents

    ```bash
    ls
    # long listing fashion
    ls -l
    # include hidden files
    ls -a
    ```

- list block device

    ```bash
    lsblk
    # list but not tree format
    lsblk -l
    ```

- check md5 sum

    ```bash
    md5sum <file-name>
    ```

- transfer and copy block file

    ```bash
    dd if=<block-file> of=<destination-path> bs=<block-size>
    sync
    ```

- unix name

    ```bash
    uname -a
    ```

- modify file access and update time if file exists else create it

    ```bash
    touch <file-name>
    ```

- change file access mode

    ```bash
    chmod <mode-in-number> <file-name>
    ```

- change file owner and group

    ```bash
    chown <owner-name>:<group-name> <file-name>
    ```

- archive file and decompress/compress file

    ```bash
    # tar: Tape Archive
    tar -zxvf abc.tar.gz
    tar -jxvf abc.tar.bz2
    ```

- calendar

    ```bash
    cal
    cal <%m> <%Y>
    ```

- standard date and time

    ```bash
    date
    ```

- concatenation files

    ```bash
    # concatenation files and print file content as standard output
    cat {1,2,3}.txt
    ```

- copy or move file

    ```bash
    cp <file-name> <path>
    mv <file-name> <path>
    ```