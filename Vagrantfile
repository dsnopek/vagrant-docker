Vagrant.configure("2") do |config|
  config.vm.box = "precise64-docker"
  config.vm.box_url = "https://oss-binaries.phusionpassenger.com/vagrant/boxes/ubuntu-12.04.3-amd64-vbox.box"
  config.vm.network :private_network, ip: "2.2.2.2"
  config.ssh.forward_agent = true
  config.vm.provision :shell, :path => "bootstrap.sh"
  config.vm.provider :virtualbox do |vb|
    vb.customize ["modifyvm", :id, "--memory", "2048"]
	vb.destroy_unused_network_interfaces = true
  end
end
