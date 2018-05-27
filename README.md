# Init
## Presentation
Introduction to sysadmin with basic UNIX commands and shell scripting.

## Getting started
### Prerequisites
* A Computer with Mac OS (no root access needed) for the `network` part.
* A Computer or VM with Debian (root access needed) for the `system` and `scripts` parts.

### Installing
Just setup a VM with debian, and get access to command line tool.
#### Setup the Debian VM easily with vagrant on 42 computers
```bash
mkdir ~/goinfre/vagrant && cd ~/goinfre/vagrant

echo 'Vagrant.configure("2") do |config|
  config.vm.box = "debian/stretch64"
  config.vm.synced_folder ".", "/git"
end
' > Vagrantfile

vagrant plugin install vagrant-vbguest && vagrant up && vagrant vbguest

vagrant ssh
```
Once in debian system
```bash
sudo passwd root
```

## Authors
* **[Thomas Bailly-Salins](https://github.com/tbailly)** - *All*
