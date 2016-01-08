Vagrant.configure(2) do |config|
  config.vm.box = "provision_rails_centos7"
  config.vm.box_url = "https://github.com/holms/vagrant-centos7-box/releases/download/7.1.1503.001/CentOS-7.1.1503-x86_64-netboot.box"
  config.vm.network "private_network", ip: "192.168.33.10"
  config.vm.provision "shell", path: "provision.sh"
  config.vm.provider "virtualbox" do |v|
    v.memory = 2048
  end
  config.vm.provision "shell", inline: "ln -s /vagrant /home/rails/vagrant"
end
