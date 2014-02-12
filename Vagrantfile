# -*- mode: ruby -*-
# # vi: set ft=ruby :

# For more info, see https://github.com/coreos/coreos-vagrant
Vagrant.configure("2") do |config|
    config.vm.box = "coreos"
    config.vm.box_url = "http://storage.core-os.net/coreos/amd64-generic/dev-channel/coreos_production_vagrant.box"

    config.vm.network "private_network", ip: "10.0.0.10"
    config.vm.synced_folder "~/working", "/home/core/working", id: "core", :nfs => true,  :mount_options => ['nolock,vers=3,udp']

    config.ssh.forward_agent = true
end
