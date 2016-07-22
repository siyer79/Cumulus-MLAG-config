#Vagrant.configure(2) do |config|
#  config.vm.box = "cumulus-vx-3.0.0" end

Vagrant.configure(2) do |config|

   config.vm.box = "cumulus-vx-3.0.0"

   
##### DEFINE VM for Switch-Leaf-1a #####
   config.vm.define "Switch-Leaf-1a" do |device|
     device.vm.hostname = "Switch-Leaf-1a"
     device.vm.network "private_network", virtualbox__intnet: "swp1"
     device.vm.network "private_network", virtualbox__intnet: "swp2"
     device.vm.network "private_network", virtualbox__intnet: "swp3"
     device.vm.network "private_network", virtualbox__intnet: "swp4"
     device.vm.network "private_network", virtualbox__intnet: "swp5"
     device.vm.network "private_network", virtualbox__intnet: "swp6"
     device.vm.network "private_network", virtualbox__intnet: "swp7"
     device.vm.network "private_network", virtualbox__intnet: "swp8"
     device.vm.network "private_network", virtualbox__intnet: "swp9"
     device.vm.network "private_network", virtualbox__intnet: "swp10"
     device.vm.network "private_network", virtualbox__intnet: "swp11"
     device.vm.network "private_network", virtualbox__intnet: "swp12"
     device.vm.network "private_network", virtualbox__intnet: "swp47"
     device.vm.network "private_network", virtualbox__intnet: "swp48"
     device.vm.network "private_network", virtualbox__intnet: "swp49"
     device.vm.network "private_network", virtualbox__intnet: "swp50"
     device.vm.network "private_network", virtualbox__intnet: "swp52"
     device.vm.network "private_network", virtualbox__intnet: "swp53" 

     device.vm.provider "virtualbox" do |v|
       v.name = "Switch-Leaf-1a"
       v.memory = 512
     end

   end

##### DEFINE VM for Switch-Leaf-1b #####
   config.vm.define "Switch-Leaf-1b" do |device|
     device.vm.hostname = "Switch-Leaf-1b"
     device.vm.network "private_network", virtualbox__intnet: "swp1"
     device.vm.network "private_network", virtualbox__intnet: "swp2"
     device.vm.network "private_network", virtualbox__intnet: "swp3"
     device.vm.network "private_network", virtualbox__intnet: "swp4"
     device.vm.network "private_network", virtualbox__intnet: "swp5"
     device.vm.network "private_network", virtualbox__intnet: "swp6"
     device.vm.network "private_network", virtualbox__intnet: "swp7"
     device.vm.network "private_network", virtualbox__intnet: "swp8"
     device.vm.network "private_network", virtualbox__intnet: "swp9"
     device.vm.network "private_network", virtualbox__intnet: "swp10"
     device.vm.network "private_network", virtualbox__intnet: "swp11"
     device.vm.network "private_network", virtualbox__intnet: "swp12"
     device.vm.network "private_network", virtualbox__intnet: "swp47"
     device.vm.network "private_network", virtualbox__intnet: "swp48"
     device.vm.network "private_network", virtualbox__intnet: "swp49"
     device.vm.network "private_network", virtualbox__intnet: "swp50"
     device.vm.network "private_network", virtualbox__intnet: "swp52"
     device.vm.network "private_network", virtualbox__intnet: "swp53"

     device.vm.provider "virtualbox" do |v|
       v.name = "Switch-Leaf-1b"
       v.memory = 512
     end

   end


   config.vm.provision "ansible" do |ansible|
     ansible.verbose = "vvv"
     ansible.playbook = "usc-leaf-playbook.yml"
   end


end



