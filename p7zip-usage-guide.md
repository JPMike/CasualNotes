### p7zip usage guide

#### install

##### Ubuntu

```bash
apt install p7zip-full
```

##### CentOS

```bash
yum -y install epel-release
yum -y install p7zip p7zip-plugins
```

#### create

```bash
7z a files.7z file{1..3}.txt
7z a files.7z files/
7z a files.zip file{1..3}.txt
```

#### list

```bash
7z l files.7z
```

#### decompress

```bash
# to current path
7z e files.7z
# to origin path
7z x files.7z
```

#### update

```bash
7z u files.7z files/
```

#### help

```bash
man 7z
```
