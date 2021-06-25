# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"
VAGRANT_IP = "10.0.0.5"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "ubuntu/focal64"
  config.vm.network :private_network, ip: VAGRANT_IP

  config.vm.synced_folder "app/", "/vagrant/app"

  # run Ansible from the Vagrant VM
  config.vm.provision "ansible_local" do |ansible|
    ansible.install = true
    ansible.playbook = ".provisioning/deploy.yml"
  end

  # add localhost to Ansible inventory
  config.vm.provision "shell", inline: "printf 'localhost\n' | sudo tee /etc/ansible/hosts > /dev/null"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "2048"
  end

end
