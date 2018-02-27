# **Code 'n Load** Official Documentation

**Code 'n Load** -CnL- is a sofware development platform designed for the Internet-of-Things (IoT). CnL allows you to manage, monitor and control parameters of your device and the software it runs. You only have to setup the CnL daemon on your device and a git repository for the software you want to execute on the device. The daemon will monitor the repository for changes and update the software if needed.

This is the official documentation repository for the alpha version.

- [User manual and getting started guide](user_manual.md): Step-by-step guide for device setup and usage of the Control Panel, which allows you to deploy software on the device, control its execution and retreive real-time status.

- [Code 'n Load User Application Format](cnl_app.md): `cnl_app` is the user application running on each device. This document describes the structure of the source code and the Makefile rules.

- [Code 'n Load daemon documentation](cnld.md): `cnld` is the daemon running on each device. Software structure, commands and configuration parameters are described in this document.
