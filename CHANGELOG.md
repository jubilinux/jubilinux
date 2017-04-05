# v0.1.1

* New kernel with patched kernel/ptrace.c to not spam dmesg/syslog/etc when the `fuser` command is run.

# v0.1.0

* edison-linux kernel 3.10.98, up from 3.10.17
* first-install.target exists so the post-flash boot sequence requires no manual intervention
* some extra sleep in /etc/rc.local before spawning bluetooth services to ensure the bluetooth stack is running

# v0.0.0

Initial release
