### shell usage guide

- generate parameter

    ```bash
    echo {a,b,c}file
    echo {a,b,c}{1,2,3}file
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