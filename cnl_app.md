# Code 'n Load User Application Format

The application you want to run on the device must have a `Makefile` on its root folder. This makefile must meet the following characteristics:

- Have an `update` rule, commonly used for compilation and daemon reload.
- Have a `clean` rule to remove all objects, binaries and other execution files.
- The final binary/executable/script file must be called `cnl_app`.

Example `Makefile` for the default C application: https://github.com/codenload/cnl_app/blob/master/Makefile

Example `Makefile` for the default Python application: https://github.com/codenload/cnl_app_py/blob/master/Makefile
