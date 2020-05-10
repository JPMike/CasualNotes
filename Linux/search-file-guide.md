### search file guide

- `which`

    ```bash
    # search executable file in PATH
    which pwd
    ```

- `whereis`

    ```bash
    # search program name with database
    whereis sshd
    # search only binary file
    whereis -b sshd
    # search only source file
    whereis -s sshd
    # search only help file
    whereis -m sshd
    ```

- `locate`

    ```bash
    # search file with database
    locate pwd
    locate /etc/sh
    ```