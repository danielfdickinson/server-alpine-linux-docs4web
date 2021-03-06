---
date: 2022-04-29
title: Prepare your SD card
tags: ["alpine","configuration","docs","linux","sysadmin-devops","raspberry-pi","sbc"]
series: ["docs4web","alpine-linux-local-server"]
description: "Prepare the filesystem of the Alpine Linux bootstrap SD card for your Raspberry Pi"
summary: "Prepare the filesystem of the Alpine Linux bootstrap SD card for your Raspberry Pi"
---

## Partition the SD card

### On Windows 10

#### Using built-in GUI 'Disk Management' feature

TBD

#### Using diskpart

TBD

#### Using PowerShell

TBD

### On Linux (many distros)

#### GUI

[Using Gnome 'Disks' applet](prepare-sd-using-gnome-disks/_index.md)

#### Using command line (CLI)

[Partitioning on the Linux command line](../../../linux-cli-partitioning/_index.md)

[Creating a filesystem on the Linux command line](../../../server-install-config/create-semi-data-install/add-and-use-filesystem-tools.md#vfatfat32fat16)

### On Mac OS

TBD

## Copy the tarball contents to 'boot' partition

### On Windows 10

You will need to install a program such a [7-zip](https://www.7-zip.org/)

TBD

### On Linux (many distros)

[Copy install tarball to boot partition using GUI file manager](copy-tarball-to-boot-under-gnome/_index.md)

#### Using CLI commands

Assuming you have mounted your new boot partition on `/mnt` you can (as root) do:

```shell
tar -C /mnt -xzf /path/to/install-tarball.tar.gz
```

### On Mac OS

TBD
