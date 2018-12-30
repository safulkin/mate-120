# mate-1.20 for Funtoo Linux 1.2
This repo contain ebuilds of **MATE Desktop Environment 1.20 stable release**.
Versions updated according http://pub.mate-desktop.org/releases/1.20/

**How to add this overlay**
- Create directory for overlay files
```
    mkdir -p /var/git/mate-120
```
- /etc/portage/repos.conf/mate-120 
    [mate-120]
    location = /var/git/mate-120
    sync-type = git
    sync-uri = https://github.com/safulkin/mate-120.git
    auto-sync = yes
    priority = 2


**Upgrade steps:**
- emerge --oneshot =mate-base/mate-common-1.20.0
- emerge --update --deep --newuse mate
