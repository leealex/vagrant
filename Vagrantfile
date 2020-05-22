# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "leealex/debian9lemp"
  config.vm.network "private_network", ip: "10.10.10.100"
  config.vm.synced_folder "../www", "/var/www", type: "virtualbox", create: true, owner: "www-data", group: "www-data"

  # Uncomment the line below to install fsnotify https://github.com/adrienkohlbecker/vagrant-fsnotify
  #config.vagrant.plugins = "vagrant-fsnotify"

  config.vm.provider "virtualbox" do |v|
    v.name = "Debian_9"
    v.customize ["modifyvm", :id, "--memory", "4096"]
  end

  config.ssh.insert_key = false

end
