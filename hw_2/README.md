
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
![Schema](docs/20230221_195400.png)

### command
```bash
$ uname -srm
# or
$ hostnamectl | grep -i "kernel"
```

# 3. List kernel modules and write to file

## Result
```bash
# check hw2/docs/mod.txt
```
### command
```bash
$ lsmod > mod.txt
# or
$ cat /proc/modules > mod.txt
# cat mod.txt
```

# 4. Display information about CPU, MEM, HDD host and VM

### command
```bash
# for CPU
$ lscpu
# for MEM
$ free -m
# for HDD
$ lsblk
```