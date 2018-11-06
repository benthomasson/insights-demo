# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.define "Host1" do |host1|
	host1.vm.box = "generic/rhel7"
    host1.vm.network :forwarded_port, id: "ssh", guest: 22, host: 2222
  end

  config.vm.define "Host2" do |host2|
	host2.vm.box = "generic/rhel7"
    host2.vm.network :forwarded_port, id: "ssh", guest: 22, host: 2200
  end
  config.vm.define "Host3" do |host3|
	host3.vm.box = "generic/rhel7"
    host3.vm.network :forwarded_port, id: "ssh", guest: 22, host: 2201
  end
  config.vm.define "Host4" do |host4|
	host4.vm.box = "generic/rhel7"
    host4.vm.network :forwarded_port, id: "ssh", guest: 22, host: 2202
  end
end
