# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure(2) do |config|
  config.vm.box = "generic/centos8s"
 
 config.vm.provider "virtualbox" do |v|
    v.memory = 2048
    v.cpus = 2
end
 
 config.vm.define "nfss" do |nfss|
    nfss.vm.network "private_network", ip: "192.168.50.10",
virtualbox__intnet: "net1"
    nfss.vm.hostname = "nfss"
    nfss.vm.provision "shell", path: "scr.sh"
end
end
