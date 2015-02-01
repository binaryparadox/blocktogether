# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure("2") do |config|
  config.vm.box = "trusty32"
  config.vm.box_url = "https://cloud-images.ubuntu.com/vagrant/trusty/current/trusty-server-cloudimg-i386-vagrant-disk1.box"
  config.vm.box_download_checksum_type = "sha256"
  config.vm.box_download_checksum = "b6d77ffc4367e7ec95f43e911a89fe425b9165e129ed64dd2c00a2c837cb9166"
  config.vm.provision :shell, privileged: false, path: "bin/vagrant_up.sh"
  config.vm.network :forwarded_port, host: 3000, guest: 3000
end