# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  # General Vagrant VM conguration.
  config.vm.box = "geerlingguy/ubuntu2004"
  config.vm.network :private_network, ip: "192.168.56.8"
  config.vm.hostname = "drupal1.test"
  config.ssh.insert_key = false
  
  config.vm.provider :virtualbox do |v|
     v.memory = 2048
  end

#  # Ansible provisioning.
#  config.vm.provision "ansible" do |ansible|
#    ansible.playbook = provisioning/playbook.yaml
#  end
end
