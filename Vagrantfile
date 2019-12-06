# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANT_API_VERSION = 2

Vagrant.configure(VAGRANT_API_VERSION) do |config|
  config.ssh.insert_key = false
  config.vm.synced_folder '.', '/vagrant', disabled: true
  config.vm.define 'mariadb' do |mariadb|
    mariadb.vm.hostname = 'mariadb'
    mariadb.vm.box = 'centos/7'
    mariadb.vm.network "private_network", ip: "192.168.56.11"
  end
  

  config.vm.provider "virtualbox" do |mariadb|
    mariadb.memory = 4096
    mariadb.cpus = 2
  end

end
