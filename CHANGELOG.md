# Changelog

## v0.2.0

* Added a ton of kernel modules, basically anything that was removable via USB or i2c.
* Added /root/kernel.config for transparency about the kernel as built.
* Install `sudo` via apt-get
* Remove galileod service and /opt/edison arduino launcher stuff
* Added `bash-completion` package
* Enable swap in kernel
* Install bluez via `apt-get install bluez`
* Install `libnss-myhostname` so that systemd-hostnamed works
* Enable all kernel namespace support
* Remove systemd-hostnamed service to avoid unnecessary errors
* Remove bluetoothd service, since it is started by rc.local

## v0.1.1

* Add `jubilinux` to `/etc/hosts` as `127.0.0.1` so tools like `sudo` stop complaining.
* New kernel with patched kernel/ptrace.c to not spam dmesg/syslog/etc when the `fuser` command is run.

# v0.1.0

* edison-linux kernel 3.10.98, up from 3.10.17
* first-install.target exists so the post-flash boot sequence requires no manual intervention
* some extra sleep in /etc/rc.local before spawning bluetooth services to ensure the bluetooth stack is running

# v0.0.0

Initial release

