# mosaicgnss-dev

My ROS driver development environment for the Septentrio Mosaic GNSS module.

## Info

- OS

```
Distributor ID: Debian
Description: Debian GNU/Linux 9.13 (stretch)
Release: 9.13
Codename: stretch
```

- g++

```
g++ (Debian 6.3.0-18+deb9u1) 6.3.0 20170516
```

- CMake

```
cmake version 3.7.2
```

## Setup

- Clone repository

```bash
git clone https://github.com/ashwin5059198/mosaicgnss-dev.git
cd mosaicgnss-dev
```

- Build required images

```bash
docker-compose build
```

- Start services

```bash
docker-compose up
```

- Run bash in a running container

In a new shell, run

```bash
./shell.sh
```

## Other

- The `shell.sh` executable script can be used a shell replacement. By default it tries to spawn a shell from a running container. If unsuccessful, it spawns a bash shell from root system instead.

eg: for VSCode, in the `settings.json` file, add the following line:

```json
{
  "terminal.integrated.shell.linux": "${workspaceFolder}/shell.sh"
}
```
