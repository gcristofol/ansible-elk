# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  # The most common configuration options are documented and commented below.
  # For a complete reference, please see the online documentation at
  # https://docs.vagrantup.com.

  # Every Vagrant development environment requires a box. You can search for
  # boxes at https://atlas.hashicorp.com/search.
  config.vm.box = "ericmann/trusty64"
  config.vm.provider "hyperv"
  config.vm.network "public_network"

  config.vm.provider "hyperv" do |vb|
     # Customize the amount of memory on the VM:
     vb.memory = "2048"
  end
  
  config.vm.provision "shell",
    inline: "echo Hello, World"
	
  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "playbook.yml"
  end
end
