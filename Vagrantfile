# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/xenial64"

  config.vm.synced_folder ".", "/vagrant"

  config.vm.provider :virtualbox do |v|
     v.customize ["modifyvm", :id, "--memory", 1048]
     v.name = "tetrifact-build"
  end

  config.vm.provision :shell, path: "provision.sh"

end
