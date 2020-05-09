### pgrep usage guide

- find pid

    ```bash
    pgrep ssh
    ```

- find pid and process name

    ```bash
    pgrep ssh -l
    ```

- specify separator

    ```bash
    pgrep ssh -l -d ,
    ```

- find with pattern

    ```bash
    pgrep '^sshd$' -l
    ```

- find with user

    ```bash
    pgrep -u root -l
    ```

- find reverse

    ```bash
    pgrep -v -u root -l
    ```

- count only

    ```bash
    pgrep -v -u root -l -c
    ```