# dokku-monit
Dokku plugin for monit monitoring of apps. Adds a monitrc file in each APP directory which can easily be included in /etc/monitrc. Also reloads monit on deploy/deletion/domain changes.

A lot of the code is based upon the nginx-vhost plugin, included with dokku.

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
