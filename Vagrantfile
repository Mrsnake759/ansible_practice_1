Vagrant.configure("2") do |config|
  config.vm.box = "tknerr/ubuntu2004-desktop"
  config.vm.hostname = "ansible-semaphore"
  config.vm.network "private_network", ip: "192.168.50.5"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
    ansible.inventory_path = "hosts.ini"
  end
end
