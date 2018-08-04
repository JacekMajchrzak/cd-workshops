# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  config.vm.define "jenkins" do |jenkins|
      jenkins.vm.box = "kwilczynski/ubuntu-16.04-docker"
      # You may wish to use a more obscure private ip, like 10.2.2.4
      jenkins.vm.network "private_network", ip: "10.0.0.200"
  end
  config.vm.define "dev" do |dev|
      dev.vm.box = "acntech/ubuntu64-dev"
      dev.vm.box_version = "1.1"
      # You may wish to use a more obscure private ip, like 10.2.2.5
      dev.vm.network "private_network", ip: "10.0.0.201"
  end
end
