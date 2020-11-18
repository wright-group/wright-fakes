# wright-fakes

This repository allows Wright Group developers to quickly stand up fake daemons and associated for pretending that they are using a certain system.
Currently only tested on Linux.

## prepare

```
$ apt install docker.io
$ apt install docker compose
```

## write appropriate yaqc-cmds config

(in directory corresponding to the system you want to mimic)

```
$ cp yaqc-cmds-config.toml ~/.config/yaqc-cmds/config.toml
```

## start daemons in docker container

(in directory corresponding to the system you want to mimic)

```
$ sudo socker-compose up --build
```

this runs the containers in the foreground, simply exit the process to stop them

local ports needed must be open before running this command

