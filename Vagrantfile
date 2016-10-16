# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "ubuntu/xenial64"

  #config.vm.synced_folder ".", "/vagrant"

  # increase memory and cpus accordingly to shorten build time
  config.vm.provider "virtualbox" do |v|
    v.memory = 8192
    v.cpus = 4
  end

  config.vm.provision "shell",
    inline: "apt-get update && apt-get install -y python-minimal unzip"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible/setup.yml"
  end

end
