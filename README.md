<!--
N.B.: This README was automatically generated by https://github.com/YunoHost/apps/tree/master/tools/README-generator
It shall NOT be edited by hand.
-->

# Funkwhale for YunoHost

[![Integration level](https://dash.yunohost.org/integration/funkwhale.svg)](https://dash.yunohost.org/appci/app/funkwhale) ![Working status](https://ci-apps.yunohost.org/ci/badges/funkwhale.status.svg) ![Maintenance status](https://ci-apps.yunohost.org/ci/badges/funkwhale.maintain.svg)  
[![Install Funkwhale with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=funkwhale)

*[Lire ce readme en français.](./README_fr.md)*

> *This package allows you to install Funkwhale quickly and simply on a YunoHost server.
If you don't have YunoHost, please consult [the guide](https://yunohost.org/#/install) to learn how to install it.*

## Overview

Funkwhale is a community-driven project that lets you listen and share music and audio within a decentralized, open network. 

**Shipped version:** 1.2.8~ynh1


**Demo:** https://demo.funkwhale.audio

## Screenshots

![Screenshot of Funkwhale](./doc/screenshots/screenshot1.png)

## Disclaimers / important information

* Installation requires a dedicated domain or subdomain. Installing in a subpath is not supported by the upstream project due to dependency requirements.

* Admin

The admin uses the login you provided at installation. The password is the same you use for YunoHost.
The admin interface is accessible at the address: `your.domain.fr/api/admin`

To add a collection of music files to a library in your YunoHost installation of Funkwhale, create a symlink to your collection titled "music" in `/home/yunohost.app/funkwhale/data`
```console
foo@bar:~$sudo ln -s /your/music/collection /home/yunohost.app/funkwhale/data/music
```
The files can then be added to your library from the *uploading* tab in a music library under the heading **Import music from your server**.

## Documentation and resources

* Official app website: <https://funkwhale.audio/>
* Official user documentation: <https://docs.funkwhale.audio/users/index.html>
* Official admin documentation: <https://docs.funkwhale.audio/admin/index.html>
* Upstream app code repository: <https://dev.funkwhale.audio/funkwhale/funkwhale>
* YunoHost documentation for this app: <https://yunohost.org/app_funkwhale>
* Report a bug: <https://github.com/YunoHost-Apps/funkwhale_ynh/issues>

## Developer info

Please send your pull request to the [testing branch](https://github.com/YunoHost-Apps/funkwhale_ynh/tree/testing).

To try the testing branch, please proceed like that.

``` bash
sudo yunohost app install https://github.com/YunoHost-Apps/funkwhale_ynh/tree/testing --debug
or
sudo yunohost app upgrade funkwhale -u https://github.com/YunoHost-Apps/funkwhale_ynh/tree/testing --debug
```

**More info regarding app packaging:** <https://yunohost.org/packaging_apps>
