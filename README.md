# ClearWSL
Clear Linux on WSL (Windows 10 x64 v2004 or later)
based on [wsldl](https://github.com/yuk7/wsldl).

![screenshot](https://raw.githubusercontent.com/wiki/yuk7/wsldl/img/Cent_Arch_Alpine.png)
[![Build Status](https://img.shields.io/travis/com/wight554/ClearWSL.svg?style=flat-square)](https://travis-ci.com/ZVNexus/ClearWSL)
[![Github All Releases](https://img.shields.io/github/downloads/wight554/ClearWSL/total.svg?style=flat-square)](https://github.com/ZVNexus/ClearWSL/releases/latest)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
![License](https://img.shields.io/github/license/wight554/ClearWSL.svg?style=flat-square)

### [Download](https://github.com/ZVNexus/ClearWSL/releases/latest)

## Requirements
* Windows 10 x64 v2004 or later.
* Windows Subsystem for Linux feature is enabled.

## Install
#### 1. [Download](https://github.com/wight554/ClearWSL/releases/latest) installer archive.

#### 2. Extract all files in archive to same directory.

#### 3. Run Clear EXE to extract ROOTFS and register to WSL.
Exe filename is used to register the instance name.
If you rename it, you can register with a different name and have multiple installs.

## How-to-Use (for installed instance).
#### EXE arguments:
```dos
Usage :
    <no args>
      - Open a new shell with your default settings.

    run <command line>
      - Run the given command line in that distro. Inherit current directory.

    config [setting [value]]
      - `--default-user <user>`: Set the default user for this distro to <USER>.
      - `--default-uid <uid>`: Set the default user uid for this distro to <UID>.
      - `--append-path <on|off>`: Switch of Append Windows PATH to $PATH.
      - `--mount-drive <on|off>`: Switch of mount drives.

    get [setting]
      - `--default-uid`: Get the default user UID in this distribution.
      - `--append-path`: Get on/off status of Append Windows PATH to $PATH.
      - `--mount-drive`: Get on/off status of mount drives.
      - `--lxuid`: Get LxUID key for this distribution.

    backup
      - Output backup.tar.gz to the current directory using tar command.
      
    clean
      - Uninstall the distribution.

    help
      - Print this usage message.
```

#### How to uninstall instance.
```dos
> Clear.exe clean
```
