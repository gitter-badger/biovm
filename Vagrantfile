Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.box_check_update = true

  config.vm.provider :virtualbox do |v, override|
    v.gui = true
    v.customize ["modifyvm", :id, "--name", "BioVM 16.04"]    
    v.customize ["modifyvm", :id, "--memory", 2048]
    v.customize ["modifyvm", :id, "--cpus", 1]
    v.customize ["modifyvm", :id, "--vram", "256"]
    v.customize ["setextradata", "global", "GUI/MaxGuestResolution", "any"]
    v.customize ["setextradata", "global", "GUI/MiniToolBarAlignment", "Top"]
    v.customize ["setextradata", :id, "CustomVideoMode1", "1366x768x32"]
    v.customize ["modifyvm", :id, "--ioapic", "on"]
    v.customize ["modifyvm", :id, "--rtcuseutc", "on"]
    v.customize ["modifyvm", :id, "--accelerate3d", "on"]
    v.customize ["modifyvm", :id, "--clipboard", "bidirectional"]
#    v.customize ["modifyvm", :id, "--uart1", "off"]        
  end
    
  config.vm.provision "ansible_local" do |a|
    a.playbook = "setup.yml"
    a.compatibility_mode = "2.0"
  end
end
