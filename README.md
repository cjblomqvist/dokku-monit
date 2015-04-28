# dokku-monit
Dokku plugin for monit monitoring of apps

## Installation
```
$ sudo su # (Required for permissions - don't use sudo - currently not needed)
# cd /var/lib/dokku/plugins
# git clone --depth 1 https://github.com/cjblomqvist/dokku-monit monit
# dokku plugins-install (currently not needed)
```

## TODO
This is still far from complete, but works as a proof of concept of how to use monit with dokku (externally). Ideally, the following would be added:
* Automatically installs monit with `dokku plugins-install` and sets /etc/monitrc properly, including access rights (including sudoers)
* More flexibility in how templates can be added
