# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.define "master" do |master|
    master.vm.box = "ubuntu/bionic64"
    master.vm.network "private_network", ip: "192.168.33.10"
    master.vm.provider "virtualbox" do |vb|
    # Display the VirtualBox GUI when booting the machine
      vb.gui = false
    # Customize the amount of memory on the VM:
      vb.memory = "6144"
    end
  end

  config.vm.define "worker" do |worker|
    worker.vm.box = "ubuntu/bionic64"
    worker.vm.network "private_network", ip: "192.168.33.11"
    worker.vm.provider "virtualbox" do |vb|
    # Display the VirtualBox GUI when booting the machine
      vb.gui = false
    # Customize the amount of memory on the VM:
      vb.memory = "6144"
    end
  end
end
