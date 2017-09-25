# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|

config.vm.define "vmone" do |vmone|
 
 vmone.vm.hostname = "benwoodhouse.qac.local"
   vmone.vm.box = "chad-thompson-VAGRANTSLASH-ubuntu-trusty64-gui"
   vmone.vm.network "public_network", ip: "192.168.1.122"
	vmone.vm.provision "shell", path: "script.sh"
	
  vmone.vm.provider "virtualbox" do |vb|
    vb.gui = true
     vb.memory = 4096
	 vb.cpus = 2
	 
   end
end

    config.vm.define "vmtwo" do |vmtwo|
	
 vmtwo.vm.hostname = "benwoodhouse.qac.local"
   vmtwo.vm.box = "chad-thompson-VAGRANTSLASH-ubuntu-trusty64-gui"
   vmtwo.vm.network "public_network", ip: "192.168.1.222"
   vmtwo.vm.provision "shell", path: "script.sh"


  vmtwo.vm.provider "virtualbox2" do |vb|
  #   # Display the VirtualBox GUI when booting the machine
    vb.gui = true
     vb.memory = 4096
	 vb.cpus = 2
	 
   end
  #
  # View the documentation for the provider you are using for more
  # information on available options.

  # Enable provisioning with a shell script. Additional provisioners such as
  # Puppet, Chef, Ansible, Salt, and Docker are also available. Please see the
  # documentation for more information about their specific syntax and use.
  
	end
end