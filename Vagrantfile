Vagrant.configure("2") do |config|

  config.vm.define "ansible1" do |ansible1|
    ansible1.vm.box = "generic/ubuntu2004"
    ansible1.vm.hostname = "ansible1"
    ansible1.vm.network "private_network", ip: "10.10.20.3"
    ansible1.vm.provider "libvirt" do |libvirt|
      libvirt.cpus = 2
      libvirt.memory = 2048
    end
  end

  config.vm.define "client11" do |client11|
    client11.vm.box = "generic/ubuntu2004"
    client11.vm.hostname = "client11"
    client11.vm.network "private_network", ip: "10.10.20.4"
    client11.vm.provider "libvirt" do |libvirt|
      libvirt.cpus = 1
      libvirt.memory = 1024
    end
  end

  config.vm.define "client22" do |client22|
    client22.vm.box = "generic/ubuntu2004"
    client22.vm.hostname = "client22"
    client22.vm.network "private_network", ip: "10.10.20.5"
    client22.vm.provider "libvirt" do |libvirt|
      libvirt.cpus = 1
      libvirt.memory = 1024
    end
  end

end
