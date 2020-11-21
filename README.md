# crosscompiler-4-windows-docker-devcontainer
vs code Devcontainer with crosscompiler to develop c programms for windows


## Use Docker-Container

Using the VSCode *Remote - Containers* extension and run "RemoteContainer: Reopen in Container"

Alternatively create docker-container from .devcontainer/Dockerfile

## Hello World

### build for linux
```
cd helloword
mkdir linux
gcc -Wall -o linux/helloworld source/helloworld.c
```
### build for Windows
```
cd helloword
mkdir windows
i686-w64-mingw32-gcc -Wall -o windows/helloworld.exe source/helloworld.c
```

## Serial

get inspiration and code :-) from 
https://github.com/sainoky/serial_port_monitor

Tip: If you wan compile serial_port_monitor from sainoky for windows use `-D_MSC_VER=1400`
### build for linux
see repository for serial port monitor

### build for windows
```
cd serial
mkdir windows
i686-w64-mingw32-gcc -o windows/serial.exe src/serial_windows.c 
```


