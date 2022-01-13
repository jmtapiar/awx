Vagrant.configure("2") do |config|
    config.vm.define "vm1" do |vm1|
        vm1.vm.box = "centos/7"
        vm1.vm.hostname = "ssh1"
        vm1.vm.provider "virtualbox" do |vb|
            vb.memory = 2048
            vb.cpus = 2
        end
        vm1.vm.network :private_network, ip: "192.168.56.10"
    end
    config.vm.define "vm2" do |vm2|
        vm2.vm.box = "centos/7"
        vm2.vm.hostname = "ssh2"
        vm2.vm.provider "virtualbox" do |vb|
            vb.memory = 2048
            vb.cpus = 2
        end
        vm2.vm.network :private_network, ip: "192.168.56.11"
        vm2.vm.synced_folder ".", "/vagrant", disabled: true
    end
    config.vm.define "vm3" do |vm3|
        vm3.vm.box = "centos/7"
        vm3.vm.hostname = "ssh3"
        vm3.vm.provider "virtualbox" do |vb|
            vb.memory = 2048
            vb.cpus = 2
        end
        vm3.vm.network :private_network, ip: "192.168.56.12"
        vm3.vm.synced_folder ".", "/vagrant", disabled: true
    end
end
