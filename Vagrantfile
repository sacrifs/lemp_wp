# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.ssh.insert_key = false
  config.vm.provider :virtalbox do |provider, override|
    provider.name = "lempwptest"
    provider.memory = 1024
  end

  config.vm.box = "bento/centos-7.1"
  config.vm.hostname = "lempwptest.dev"
  config.vm.network :private_network, ip: "192.168.10.13"

  config.vm.synced_folder ".", "/vagrant", mount_options:["dmode=777", "fmode=666"]
end
