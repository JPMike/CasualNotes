### shell usage guide

- generate parameter

    ```bash
    echo {a,b,c}file
    echo {a,b,c}{1,2,3}file
    echo file{1..10}
    cp /path-to-some-file/file{,.bak}
    rm file{1,2,3}.txt
    mv *.{c,cpp} src/
    ```

- access path

    ```bash
    # current path
    pwd
    # go home
    cd
    # go back last path
    cd -
    # last command path
    /usr/bin/script.sh
    chmod +x !$
    # last command all path
    file script{1,2,3}.sh
    chomd +x !*
    ```

- duplicate command

    ```bash
    # last command
    apt install net-tools
    sudo !!
    # histroy command
    history | grep 'config'
    !<history-command-id>
    # short cut for history
    his()
    {
        history | grep "$@"
    }
    ```

- auto yes

    ```bash
    yes | your-command
    ```

- last command return value

    ```bash
    #!/bin/bash
    filename=$1
    tail | grep 'next' $filename
    [$? -ne 0 ] && { do-something }
    ```

- current process id

    ```bash
    $$
    ```

- delete command hot key

    delete before cursor: `Ctrl+u`

    delete after cursor: `Ctrl+k`

- move cursor

    move to front: `Ctrl+a`

    move to back: `Ctrl+e`

- list operation

    ```bash
    # define
    a=(1 2 3 4 5)
    echo $a
    # get length
    echo ${#a[@]}
    echo ${#a[*]}
    # read
    echo ${a[2]}
    echo ${a[*]}
    # assign
    a[1]=100
    # delete
    unset a[1]
    unset a
    # slice
    echo ${a[*]:0:2}
    c=(${a[*]:1:3})
    # substitute
    echo ${a[*]/3/100}
    ```

