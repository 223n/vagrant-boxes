# Packer Template Debian, CentOS, Windows Vagrant box

## Requiment

- [Vagrant](http://www.vagrantup.com/ "Vagrant")
- [Packer](http://www.packer.io/ "Packer")
- [Oracle VM VirtualBox](https://www.virtualbox.org/ "Oracle VM VirtualBox")

## building Debian Vagrant box

### Debian 9

```shell
packer build debian-9.json
```

### CentOS 7

```shell
packer build centos-7.json
```

### Windows 10

```shell
packer build windows_10.json
```

## Test

```shell
ansible-galaxy install -p ./roles -r requirements.yml --force
vagrant up
```
