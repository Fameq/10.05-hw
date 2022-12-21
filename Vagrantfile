Vagrant.configure("2") do |config|

config.vm.define "master" do |master|
  master.vm.box = "ubuntu"
  master.vm.hostname = "master-node"
  master.vm.network "public_network", ip: "192.168.0.100"
  master.vm.provider "virtualbox" do |vb|
      vb.memory = 4048
      vb.cpus = 2
  end
end
end
