# WLinux

A Linux distribution optimized for WSL based on Debian stable.

## Features Overview

- Optimized for use with Windows Subsystem for Linux on Windows 10.
- Out-of-the-box support for external Windows X clients, such as [X410](https://www.microsoft.com/store/productId/9NLP712ZMN9Q).
- Several useful packages are pre-installed, including git and python3. Additional packages can be easily installed via the apt package management system.
- A handful of unnecessary packages, such as systemd and iptables, have been removed to improve stability and security.
- Scripts to easily install the following popular applications:
    - Visual Studio Code `$ sudo /opt/installcode.sh`
    - Google Chrome `$ sudo /opt/installchrome.sh`

## User Support

### WSL Resources

See [Awesome WSL](https://github.com/sirredbeard/Awesome-WSL) for a comprehensive overview of WSL.

### Getting Help 

First search for your issue [here](https://github.com/sirredbeard/WLinux/issues). If you are unable to find help, please open an issue [here](https://github.com/sirredbeard/WLinux/issues/new).

## Background

WLinux is a Linux distro optimized for use on Windows Subsystem for Linux (WSL). While other distros are availablw for WSL, this is the first Linux distro specifically designed for use on WSL. A number of enhancements are enabled by default and additional improvements are planned.

WLinux is open-source and based on the stable Debian release. Development occurs on GitHub. Pull requests, forks, and issue reports are welcomed. A paid version of WLinux is planned for the Microsoft Store to support ongoing development.

Note: There are no .iso or .img files available for WLinux, only a tar.gz image for use on Windows Subsystem for Linux.

## Project Progress

Completed:

    - Custom Linux distro image based on Debian stretch build working.
    - Custom create-targz.sh script forked from Debian's upstream version.
    - Custom /etc/os-release for Xebian.
    - Custom /etc/profile optimized for WSL.
    - Custom /etc/apt/sources.list for Xebian.
    - Scripts to install popular software:
        - Google Chrome
        - Microsoft Virtual Studio Code
    - Support for Windows X clients (via settings in /etc/profile)
    - Pre-install git and python3.
    - Remove systemd and iptables.

To Do:

    - Complete branding.
    - Complete Windows app containerization.
    - Custom color theme.
    - Additional third-party app install scripts planned:
        - Oracle Java
        - Anaconda

## Project Components

- create-targz.sh - Builds the WLinux custom Linux distro in a Debian environment.
- Launcher project - Builds the actual executable that is run when a user launches the app.
- DistroLauncher-Appx project - Builds the distro package with all the assets and other dependencies.

Read more about the components [here](https://github.com/Microsoft/WSL-DistroLauncher). 

## Related Pages

- [Awesome WSL](https://github.com/sirredbeard/Awesome-WSL)
- [Awesome UNIX](https://github.com/sirredbeard/Awesome-UNIX)

## Intellectual Property Compliance

- UNIX® is a trademark of The Open Group.
- Debian® is a registered trademark of Software in the Public Interest, Inc.
- Microsoft®, Microsoft Store®, Windows 10®, Visual Studio®, and Xenix® are trademarks or registered trademarks of Microsoft Corporation.
- Linux® is a registered trademark of Linus Torvalds.
- Chrome™ is a registered trademarks of Alphabet, Inc.