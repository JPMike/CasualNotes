### docker usage guide

- [install on ubuntu](https://docs.docker.com/install/linux/docker-ce/ubuntu/)

- user docker through none root user

    ```bash
    sudo usermod -aG docker <username>
    # check
    cat /etc/group | grep docker
    ```

- add registry mirrors

    `/etc/docker/daemon.json`

    ```json
    {
        "registry-mirrors": [
            "https://registry.docker-cn.com",
            "https://dockerhub.azk8s.cn",
            "https://docker.mirrors.ustc.edu.cn"
        ]
    }
    ```

    ```bash
    sudo systemctl daemon-reload
    sudo systemctl restart docker
    # check
    docker system info
    ```

- show docker system info

    ```bash
    docker system info
    ```