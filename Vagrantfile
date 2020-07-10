
Vagrant.configure("2") do |config|
  config.vm.box = "debian/buster64"
  config.vm.network "public_network", ip: "192.168.1.10" 
  config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.provision "ansible" do |ansible|
   ansible.playbook = "simple-webapp.yml"
  end
end