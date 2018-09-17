# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "fedora/28-cloud-base"
  config.vm.hostname = "ansible-training"
  config.vm.synced_folder "./", "/opt/ansible-training"

  config.vm.provision "shell", inline: <<-SHELL
    dnf -y install git vim wget
    cd /opt
    wget https://releases.ansible.com/ansible/rpm/release/epel-7-x86_64/ansible-2.5.5-1.el7.ans.noarch.rpm
    dnf localinstall -y ansible-2.5.5-1.el7.ans.noarch.rpm
  SHELL
end
