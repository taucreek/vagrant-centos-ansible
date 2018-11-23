# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "bento/centos-7.5"

  # https://www.vagrantup.com/docs/provisioning/ansible_local.html
  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "playbook.yml"
    ansible.install_mode = "pip"
    ansible.version = "2.7.2"
  end

end