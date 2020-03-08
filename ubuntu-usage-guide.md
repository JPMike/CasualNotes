### ubuntu usage guide

- [mirror list](http://mirrors.ubuntu.com/)

    country code can be found here

- select the fastest apt source in your country

    use [apt-select](https://github.com/jblakeman/apt-select)

- install python venv

    ```bash
    apt install python3-venv
    ```

- install development tools

    ```bash
    apt install build-essential
    ```

    check with:
    
    ```bash
    gcc --version
    make --version
    ```

- where is apt source list

    ```bash
    /etc/apt/sources.list
    ```

- switch to root user

    ```bash
    sudo -s
    ```