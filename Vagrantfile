Vagrant.configure("2") do |config|
  
    config.vm.box = "ubuntu/trusty64"

    config.vm.provider "virtualbox" do |v|
        v.memory = 1024
    end

    config.vm.define "wordpress" do |m|
        m.vm.network "private_network", ip: "11.168.0.55"
    end

    config.vm.define "mysql" do |m|
        m.vm.network "private_network", ip: "11.168.0.57"
    end
end