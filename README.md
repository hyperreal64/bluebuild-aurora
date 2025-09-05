# bluebuild-aurora

This is my custom build of UBlue OS Aurora. It isn't anything remarkable.

## Features

* [Aurora features](https://docs.getaurora.dev#features)
* borgmatic
* btrfs-assistant
* nmap
* Prometheus node-exporter

In contrast to the default Aurora settings, the following systemd units are disabled by default in this build:

* bluetooth.service
* cups.service
* wpa_supplicant.service
* zfs-mount.service
* zfs-share.service
* zfs-zed.service

## Installation

```shell
sudo bootc switch --enforce-container-sigpolicy ghcr.io/hyperreal64/bluebuild-aurora:latest
sudo systemctl reboot
```
