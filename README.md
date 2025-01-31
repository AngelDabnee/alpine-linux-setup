# alpine-linux-setup
Alpine Linux Setup

# Alpine Linux
## Base Installation
* download iso from internet

[https://dl-cdn.alpinelinux.org/alpine/v3.15/releases/x86_64/](https://dl-cdn.alpinelinux.org/alpine/v3.15/releases/x86_64/)

* Create a linux vm, add the ISO and boot
* type root without password to go to the linux live
* execute `setup-alpine` script to install, typing steps properly
* `reboot`

## Auto Personalization (web apps)
* login as `root`
* `apk add git`
* `git clone https://github.com/ivanchenoweth/alpine-linux-setup`
* `cd alpine-linux-setup`
* `git checkout headless-noroot`
* `./setup.sh`
* you will type twice noroot password while installing ...
* `cd ..`
* `rm -rf alpine-linux-setup`
* `reboot`

## To create dev containers:
* `git clone https://github.com/ivanchenoweth/alpine-linux-setup`
* `cd alpine-linux-setup`

## Execute code-server container
* `git checkout headless-noroot`
* `cd dev-containers`
* `./code-server.sh`

## Manual Personalization for branches w/noroot rootless user 
* login as `noroot`
* `ssh-keygen`


````
eval `ssh-agent -s`
ssh-add
````

## YouTube Video where I was based:
* https://youtu.be/X_T-cKum8dc
* ![imagen](https://github.com/AngelDabnee/alpine-linux-setup/assets/114833669/9f9a4f0b-f484-4c0a-847b-3d6349316041)

