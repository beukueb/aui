# Archlinux U Install

Install and configure archlinux has never been easier!

You can try it first with a `virtualbox`

This is a forked/mutated version of helmuthdu's original [aui](https://github.com/helmuthdu/aui)

The focus here is more a quick automatic install, where you check the scripts first for some variable setup and comment things you do not want to install. aui's original scripts are still present when you want a more customized install.

## Prerequisites

- A working internet connection
- Logged in as 'root' on the Arch LiveCD

## Basic install

    loadkeys be-latin1 #Or whatever you need
    pacman -Sy
    pacman -S git
    git clone https://www.github.com/beukueb/aui
    $editor aui/prep #To customize options in the script
    aui/prep #To execute
    reboot

## Extra packages

    aui/autoSetup systemUtilities
    aui/autoSetup -h #To see other modules you might like to install

If a certain module has programs you do not want installed, comment them out in the script.

