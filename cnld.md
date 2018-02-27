# Code 'n Load daemon

## Current commands

If you're using the Control Panel, you can send the following commands directly to the device. If accessing via SSH, you need to prepend `cnl` to the command.

- `blinkme` temporarily blinks the built-in LED of the device. It allows you to identify a device.
- `clean` execute `make clean` on the application repository.
- `clone` clone application repository.
- `coretemp` get CPU temperature.
- `config set|get` set or get configuration parameters (environment varibles in `/etc/cnl.conf`).
- `journal app|cnld|ssh` see journal log for application, daemon or ssh connection.
- `monitor on|off` enables|disables the application repository monitor. Remember to `config set CNL_APP_MONITOR_TIME=0` in order to disable monitor permanently.
- `pubkey` get public key of the device.
- `pull` execute `git pull` on the application source folder.
- `remove` remove application source code repository from device (execute `rm -rf $CNL_APP_PATH`).
- `serial` get serial number from device.
- `start` start application daemon (`systemctl start cnl_app`).
- `status [app|cnld|ssh]`
- `stop` stop application daemon (`systemctl stop cnl_app`).
- `update` execute `make update` on the application repository.

## Current configuration variables

Configuration variables are stored in `/etc/cnl.conf`.

- `CNL_PATH` path for the CnL daemon source code repository.
- `CNL_APP_URL` URL or SSH access for the application repository.
- `CNL_APP_PATH` local path for the application source code repository.
- `CNL_APP_MONITOR_TIME` monitoring time in seconds for the application repository.
- `CNL_SSH_KEY` location of the SSH keys.
- `AUTOSSH_GATETIME=0` always set to zero for `autossh`.
- `CNL_SSH_LOCAL_PORT` port number where sshd listens on the device.
- `CNL_SSH_SERVER_URL` server URL, set during device registration.
- `CNL_SSH_SERVER_PORT` server SSH port, set during device registration.
- `CNL_SSH_USER` server SSH user, set during device registration.
- `CNL_SSH_REMOTE_PORT` SSH tunnel port on server, set during device registration.