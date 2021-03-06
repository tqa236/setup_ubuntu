# Distro hopping challenge

Here's the rule:

1. Install a new distro
2. Install Terminator
3. Install zsh with its supporting packages (git, autosuggestions)
4. Setup Atom and relevant packages
5. Install Docker
3. Solve 1 exercise for each language on Exercism
4. Update to dev version
5. Repeat 2-3

## Challenges

1. Set up OpenGL Utility Toolkit (GLUT) and Codeblocks on Linux 

Ref: https://dev.to/didiksupriadi41/set-up-opengl-utility-toolkit-glut-and-codeblocks-on-linux-la3

2. Setup Atom + all packages and solve a coding exercise

3. Run Jupyter Notebook inside Docker
* Install Docker (https://docs.docker.com/engine/install/)
* Run Docker without sudo (https://docs.docker.com/engine/security/rootless/)
* Run Jupyter Notebook inside Docker

5. plaidml

6. mlflow

7. Set up a Jupyter Hub server that allows multiple users to use at the same time.

## Common

1. Use UNetbootin to prepare the installation USB (http://unetbootin.github.io/)

Error: exf remove disks or other media press any key to restart

2. Use Rufus to prepare the installation USB (https://rufus.ie/)

## Ubuntu (02/02/2020)

1. [OpenGL setup for code::blocks “cannot find -lXxf86vm”](https://stackoverflow.com/questions/12186494/opengl-setup-for-codeblocks-cannot-find-lxxf86vm)

```console
sudo apt install libxxf86vm-dev
```

## Debian (31/01/2021)

1. Graphical Debian Installer

2. Debian Installer

3. Install nonfree software/firmware

Add to `/etc/apt/sources.list` (https://unix.stackexchange.com/questions/467027/apt-refusing-to-install-kernel-firmware-package-from-debian-backports)

```
deb http://deb.debian.org/debian stretch main contrib non-free

deb http://deb.debian.org/debian-security/ stretch/updates main contrib non-free

deb http://deb.debian.org/debian stretch-updates main contrib non-free

### backports###

deb http://ftp.debian.org/debian stretch-backports main contrib non-free
```

Search for mission firmware (install `apt-file` if necessary) (https://unix.stackexchange.com/questions/556946/possible-missing-firmware-lib-firmware-i915-for-module-i915)

```
apt-file search bxt_dmc
```
