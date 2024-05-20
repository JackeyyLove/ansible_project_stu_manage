# Vagrantfile

Vagrant.configure("2") do |config|
  # Define the first VM
  config.vm.define "vm1" do |vm1|
    vm1.vm.box = "ubuntu/focal64"
    vm1.vm.network "private_network", ip: "10.32.3.131"
    vm1.vm.provider "virtualbox" do |vb|
      vb.name = "vm1"
      vb.memory = "2048"
      vb.cpus = 2
    end
  end

  # Define the second VM
  config.vm.define "vm2" do |vm2|
    vm2.vm.box = "ubuntu/focal64"
    vm2.vm.network "private_network", ip: "10.32.3.132"
    vm2.vm.provider "virtualbox" do |vb|
      vb.name = "vm2"
      vb.memory = "1024"
      vb.cpus = 1
    end
  end
end

