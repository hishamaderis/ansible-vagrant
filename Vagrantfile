Vagrant.configure("2") do |config|

  config.vm.define "anserver" do |anserver|
    anserver.vm.box = "ubuntu22.04 " #Setting machine type
	anserver.vm.network "private_network", ip: "192.168.33.22" #Set static IP
	anserver.vm.provider "virtualbox" do |vb| #Set Memory and CPUs
    vb.memory = "2048"
	vb.cpus = 1
   end
  end

  config.vm.define "anhost1" do |anhost1| #VM No'2
    anhost1.vm.box = "ubuntu22.04" #Setting machine type
	anhost1.vm.network "private_network", ip: "192.168.33.23" #Set static IP
	anhost1.vm.provider "virtualbox" do |vb| #Set Memory and CPUs
    vb.memory = "2048"
	vb.cpus = 1
   end
  end
end
# reference: https://www.agilequalitymadeeasy.com/post/vagrant-creating-multi-vms
