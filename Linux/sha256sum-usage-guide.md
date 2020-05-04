### sha256sum usage guide

compute and check SHA256 message digest

- `-b, --binary`

    read in binary mode

- `-t, --text`

    read in text mode (default)

- `-c, --check`

    read SHA256 sums from the FILEs and check them

    ```bash
    # First download the SHA256SUMS and SHA256SUMS.gpg files to the same directory as the iso
    cd download_directory
    sha256sum -c SHA256SUMS 2>&1 | grep OK
    ```