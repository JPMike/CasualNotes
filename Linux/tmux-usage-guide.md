### tmux usage guide

- install

    - Arch

        ```bash
        pacman -S tmux
        ```

    - Ubuntu / Debian

        ```bash
        apt install tmux
        ```

    - CentOS

        ```bash
        yum install tmux
        ```

- start

    ```bash
    tmux
    ```

- detach

    ```
    Ctrl+b d
    ```

- restore

    ```bash
    tmux attach
    ```

- create new session with name

    ```bash
    tmux new -s test
    ```

- attach to named detached tmux session

    ```bash
    tmux a -t test
    ```

- display tmux sessions

    ```bash
    tmux ls
    ```

- rename session

    ```
    Ctrl+b $
    ```

- switch session

    ```
    Ctrl+b s
    ```

- help

    ```
    Ctrl+b ?
    ```

- create new window

    ```
    Ctrl+b c
    ```

- destroy window

    ```
    Ctrl+b x
    ```

- switch between windows

    ```
    Ctrl+b [0-9]
    Ctrl+b Arrows
    ```

- split windows horizontally

    ```
    Ctrl+b %
    ```

- split windows vertically

    ```
    Ctrl+b "
    ```