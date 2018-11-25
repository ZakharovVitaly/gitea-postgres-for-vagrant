# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "generic/debian9"
  config.vm.network :private_network, :adapter=>1, type: "dhcp", virtualbox_intnet: true, virtualbox__intnet: "NatNetwork"
  config.vm.provider "virtualbox" do |box|
    box.name = "gitea-postgres"
    box.gui = true
    box.customize ["modifyvm", :id, "--memory", 2048]
    box.customize ["modifyvm", :id, "--cpus", 1]
  end
end
