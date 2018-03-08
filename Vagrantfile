# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.ssh.insert_key = false
  config.vm.define :rabbit1 do |rabbit1|
    rabbit1.vm.box = "centos1706_v0.3.0"
    rabbit1.vm.network :private_network, ip: "192.168.56.101"
   # rabbit1.vm.network "public_network", bridge: "eno1", ip:"192.168.131.50", netmask: "255.255.255.0"
    rabbit1.vm.provider :virtualbox do |vb|
      vb.customize ["modifyvm", :id, "--memory", "512","--cpus", "1", "--name", "rabbit1" ]
    end
  end
  config.vm.define :rabbit2 do |rabbit2|
    rabbit2.vm.box = "centos1706_v0.3.0"
    rabbit2.vm.network :private_network, ip: "192.168.56.102"
   # rabbit2.vm.network "public_network", bridge: "eno1", ip:"192.168.131.55", netmask: "255.255.255.0"
    rabbit2.vm.provider :virtualbox do |vb|
      vb.customize ["modifyvm", :id, "--memory", "512","--cpus", "1", "--name", "rabbit2" ]
    end
  end
  config.vm.define :rabbit3 do |rabbit3|
    rabbit3.vm.box = "centos1706_v0.3.0"
    rabbit3.vm.network :private_network, ip: "192.168.56.103"
   # rabbit3.vm.network "public_network", bridge: "eno1", ip:"192.168.131.55", netmask: "255.255.255.0"
    rabbit3.vm.provider :virtualbox do |vb|
      vb.customize ["modifyvm", :id, "--memory", "512","--cpus", "1", "--name", "rabbit3" ]
    end
  end
end
