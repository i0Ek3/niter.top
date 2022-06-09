+++

author = "i0Ek3"
date = "2022-05-21"
title = "Multi-host Development on macOS(Monterey) with Parallels Desktop" 
tags = [
    "Development",
]
categories = [
    "BG",
]

+++



I have two computers(Linux Laptop and macOS Desktop) and I'm lazy, I don't want to take out my laptop, so I decided to install Ubuntu 22.04 on my macOS with PD and use SSH to connect this virtual machine to development with different GitHub account, that's awesome and convient.

Here’s thing.

### Install PD on macOS

Download it from official site, and then buy it or use Trial version for 14 days.

### Install Ubuntu 22.04 on PD

Normal installation process, that's much faster than VMware Fusion.

The process of the other OS same as this way.

### Setup SSH on Ubuntu 22.04

Execute the following commands to support ssh functionality:

```Shell
# login Ubuntu 22.04
$ sudo apt update ; sudo apt upgrade # update resource
$ sudo apt install -y net-tools      # install ifconfig
$ ifconfig                           # check and record inet address
$ sudo apt install -y openssh-client openssh-server # install openssh
$ sudo ssh-keygen -A                                # generate ssh-key
$ sudo /etc/init.d/ssh start                        # enable ssh service
```

After then, you can connect your virtual machine by SSH.

### Use SSH to Connect Virtual Machine

You can choose SSH tool like Termius or default terminal to connect vritual machine easily. 

For example, run command `ssh vm_username@inet_address` from your terminal, and then type "yes", you will connected.

![](https://cdn.jsdelivr.net/gh/i0Ek3/apichost@main/niter.top/test@test.jpg)


### Further

Setup your Linux development environment, you can check this [repo](https://github.com/i0Ek3/meshell).
