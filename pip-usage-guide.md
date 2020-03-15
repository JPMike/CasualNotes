### pip usage guide

- [config file](https://pip.pypa.io/en/stable/user_guide/#config-file)

    - Per-user

        unix: `$HOME/.config/pip/pip.conf`
        
        unix(legacy): `$HOME/.pip/pip.conf`

    - Inside a virtualenv

        unix: `$VIRTUAL_ENV/pip.conf`

    - Site-wide

        unix: `/etc/pip.conf`

    - example

        ```
        [global]
        timeout = 60
        index-url = https://download.zope.org/ppix
        ```

- `show`

    To show details about an installed package

- `list`

    To list installed packages

- `list --outdated`

    To list outdated packages, and show the latest version available

- `uninstall`

- `install`

    pip supports installing from PyPI, version control, local projects, and directly from distribution files

    ```bash
    pip install SomePackage            # latest version
    pip install SomePackage==1.0.4     # specific version
    pip install 'SomePackage>=1.0.4'     # minimum version
    ```

- requirements.txt

    Requirements files are used to hold the result from pip freeze for the purpose of achieving repeatable installations

    ```bash
    pip freeze > requirements.txt
    pip install -r requirements.txt
    ```