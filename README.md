# docker-pxe - a Docker container running a continuous PXE server

# DOCKER HUB

https://registry.hub.docker.com/u/mcandre/docker-pxe/

# EXAMPLE

```
$ docker run -d -p 69:69/udp --cap-add=NET_ADMIN mcandre/docker-pxe
$ qemu-system-x86_64 -no-acpi -boot n -bootp tftp://$(boot2docker ip)/pxelinux.0
```

# REQUIREMENTS

* [Docker](https://www.docker.com/)
* [qemu](http://wiki.qemu.org/Main_Page)

## Optional

* [make](http://www.gnu.org/software/make/)

## Debian/Ubuntu

```
$ sudo apt-get install docker.io qemu
```

## RedHat/Fedora/CentOS

```
$ sudo yum install docker-io qemu
```

## non-Linux

* [VirtualBox](https://www.virtualbox.org/)
* [Vagrant](https://www.vagrantup.com/)
* [boot2docker](http://boot2docker.io/)

### Mac OS X

* [Xcode](http://itunes.apple.com/us/app/xcode/id497799835?ls=1&mt=12)
* [Homebrew](http://brew.sh/)
* [brew-cask](http://caskroom.io/)

```
$ brew cask install virtualbox vagrant
$ brew install boot2docker qemu
```

### Windows

* [Chocolatey](https://chocolatey.org/)

```
> chocolatey install docker qemu
```
