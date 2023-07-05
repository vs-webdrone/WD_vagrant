# Basic Vagrant config (API version 2)
Vagrant.configure(2) do |config|
  config.vm.box = "debian/bookworm64"
  config.vm.define "wd_test" do |rpi|
  end

  config.vm.provider "virtualbox" do |vb|
      # Customize the amount of memory on the VM:
      # vb.memory = "512" #default value for rasp
      vb.memory = "1024" # lets optimize it to make it faster
      vb.cpus = 2 
      # max cpu usage for host is limited to 60% :
      vb.customize ["modifyvm", :id, "--cpuexecutioncap", "60"]
  end

  # config.vm.provision "shell", inline: <<-SHELL
  #     cd /home/vagrant
  #     chmod ugo+x /vagrant/*.sh
  #     /vagrant/provision1.sh
  #     /vagrant/provision2.sh
  #     /vagrant/provision3.sh
  #     echo "ready! now you can do vagrant ssh, then /vagrant/run.sh, then in another console vagrant ssh and then /vagrant/ssh.sh"
  # SHELL
end