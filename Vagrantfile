# -*- mode: ruby -*-
# vi: set ft=ruby :
VAGRANT_VERSION = 2
Vagrant.configure(VAGRANT_VERSION) do |config|
	config.vm.define "imaging-packages" do |server|
		#server.vm.box = "hashicorp/precise64"
		server.vm.box = "chef/ubuntu-14.04"
		server.vm.hostname = "imaging-packages"
		server.vm.provision :ansible do |ansible|
			ansible.playbook = "test.yml"
		end
	end
end
