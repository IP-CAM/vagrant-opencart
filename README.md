bogdanbrudiu/opencart-vagrant
============================

This repository allows you to setup an OpenCart install using
vagrant for development and testing.

# Requirements

* [Virtual Box](https://www.virtualbox.org/)
* [Vagrant](http://www.vagrantup.com/)

# Installation

```bash
git clone --recursive https://github.com/bogdanbrudiu/vagrant-opencart.git
cd vagrant-opencart
git submodule init
git submodule update
```

For a specific Opencart version:

```bash
cd web
git tag -l
git checkout tags/1.5.6.4
```

Start the VM:

```bash
vagrant up
```




Open your browser to 127.0.0.1:8080 and go through the OpenCart installation
wizard.

# Configuration

This setup will install mysql and create the database for you. During the
OpenCart install, it will ask for your database information. There is
no password and the username is `root`. The database name is `opencart`
