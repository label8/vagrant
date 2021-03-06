# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|

  config.ssh.private_key_path = "~/.ssh/id_rsa"

  config.vm.define :deploy do |node|
    node.vm.box = "eighty8/ubuntu16.04-min"
    node.vm.network :forwarded_port, guest: 22, host: 2010, id: "ssh"
    node.vm.network "private_network", ip: "192.168.1.10"
  end

  config.vm.define :dev_web do |node|
    node.vm.box = "eighty8/ubuntu16.04-min"
    node.vm.network :forwarded_port, guest: 22, host: 2015, id: "ssh"
    node.vm.network "private_network", ip: "192.168.1.15"
  end

  config.vm.define :stg_web do |node|
    node.vm.box = "eighty8/ubuntu16.04-min"
    node.vm.network :forwarded_port, guest: 22, host: 2016, id: "ssh"
    node.vm.network "private_network", ip: "192.168.1.16"
  end

  config.vm.define :front do |node|
    node.vm.box = "eighty8/ubuntu16.04-min"
    node.vm.network :forwarded_port, guest: 22, host: 2020, id: "ssh"
    node.vm.network "private_network", ip: "192.168.1.20"
  end

  config.vm.define :web1 do |node|
    node.vm.box = "eighty8/ubuntu16.04-min"
    node.vm.network :forwarded_port, guest: 22, host: 2021, id: "ssh"
    node.vm.network "private_network", ip: "192.168.1.21"
  end

  config.vm.define :web2 do |node|
    node.vm.box = "eighty8/ubuntu16.04-min"
    node.vm.network :forwarded_port, guest: 22, host: 2022, id: "ssh"
    node.vm.network "private_network", ip: "192.168.1.22"
  end

  config.vm.define :dev_db do |node|
    node.vm.box = "eighty8/ubuntu16.04-min"
    node.vm.network :forwarded_port, guest: 22, host: 2040, id: "ssh"
    node.vm.network "private_network", ip: "192.168.1.40"
  end

  config.vm.define :dbm do |node|
    node.vm.box = "eighty8/ubuntu16.04-min"
    node.vm.network :forwarded_port, guest: 22, host: 2050, id: "ssh"
    node.vm.network "private_network", ip: "192.168.1.50"
  end

  config.vm.define :dbs do |node|
    node.vm.box = "eighty8/ubuntu16.04-min"
    node.vm.network :forwarded_port, guest: 22, host: 2051, id: "ssh"
    node.vm.network "private_network", ip: "192.168.1.51"
  end

end
