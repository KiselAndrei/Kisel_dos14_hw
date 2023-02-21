
# 1. Change MOTD on VM
## Result
![Schema](docs/20230221_184121.png)

## How it do

### Turn off default MOTD
```bash
$ vi /etc/default/motd-news

# Turn off default MOTD
$ ENABLED=0
```
### Edit settings

Then create ``.env`` file form the sample and edit:
```bash
cp ./internal/config/.env.sample .env
```

# 2. Define the exact kernel version
## Result
```bash
# chec hw2/docs/mod.txt
```

### command
```bash
$ uname -srm
# or
$ hostnamectl | grep -i "kernel"
# chec hw2/docs/mod.txt
```

# 3. List kernel modules and write to file


### command
```bash
$ lsmod > mod.txt
# or
$ cat /proc/modules > mod.txt
```