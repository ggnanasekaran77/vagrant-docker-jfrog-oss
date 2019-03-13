Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.network "forwarded_port", guest: 8081, host: 8081, host_ip: "192.168.33.11"
  config.vm.network "private_network", ip: "192.168.33.11"
  config.vm.provider "virtualbox" do |vb|
    vb.memory = "2048"
  end
  config.vm.provision "docker"
end

