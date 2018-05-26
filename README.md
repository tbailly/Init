# Init
Introduction to sysadmin with basic commands and shell scripting
The `network` exercices must be realized in Mac OS command line without root access.
The `system` and `scripts` part must be realized in Debian command line

##### Setup the Debian VM easily with vagrant on 42 computers
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
##### Once in debian system
```bash
sudo passwd root
```
