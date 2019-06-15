Vagrant.configure(2) do |config|

  config.vm.box = "ubuntu/xenial64"
  config.vm.network 'forwarded_port', guest: 3000, host: 3000
  config.vm.network 'forwarded_port', guest: 5432, host: 5432
  config.vm.network 'forwarded_port', guest: 9999, host: 9999
  config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.network "forwarded_port", guest: 443, host: 8443

  config.vm.provider "virtualbox" do |v|
    v.memory = 1024
    v.cpus = 1
  end

  end
