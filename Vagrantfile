# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
    config.ssh.forward_x11 = true
    config.ssh.forward_agent = true
    config.vm.network "forwarded_port", guest: 8080, host: 8080, auto_correct: true

    config.vm.define "jenkinstest" do |jenkinstest|
        jenkinstest.vm.hostname = "jenkinstest"
        jenkinstest.vm.box = "trusty-server"
        jenkinstest.vm.box_url = "https://oss-binaries.phusionpassenger.com/vagrant/boxes/latest/ubuntu-14.04-amd64-vbox.box"

        jenkinstest.vm.provision "ansible" do |ansible|
            ansible.playbook = "ansible/provision.yml"
            ansible.sudo = "True"
            ansible.verbose = "vvvv"
        end
    end
end
