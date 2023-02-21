
# 1. Change MOTD on VM

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
![Schema](docs/20230221_195400.png)

### command
```bash
$ uname -srm
# or
$ hostnamectl | grep -i "kernel"
```

# 3. Define the exact kernel version
![Schema](mod.txt)

### command
```bash
$ uname -srm
# or
$ hostnamectl | grep -i "kernel"
```