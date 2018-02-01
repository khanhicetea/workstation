# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "https://cloud-images.ubuntu.com/xenial/current/xenial-server-cloudimg-amd64-vagrant.box"
  config.vm.box_check_update = false
  config.vm.network "private_network", ip: "192.168.111.111"

  config.vm.provider "virtualbox" do |vb|
    vb.name = "workstation"
    vb.cpus = 2
    vb.memory = 2048
  end

  config.vm.provision "shell", inline: "sudo apt -y install python-simplejson"
end
