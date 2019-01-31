centos-packer
=============

CentOS 7 x64 + VirtualBox / VMWare for Packer Template

## Packer Build for VirtualBox

```
cd centos7
packer validate CentOS_7.json 
VERSION=v1.0.0.0 packer build [ -only virtualbox-iso | -only vmware-iso ] CentOS_7.json
```

## Add Vagrant Box

```
vagrant box add BOXNAME CentOS-7-x86_64-v1.0.0.0-virtualbox.box
or
vagrant box add BOXNAME CentOS-7-x86_64-v1.0.0.0-vmware.box
```

