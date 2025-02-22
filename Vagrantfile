Vagrant.configure("2") do |config|
  
  config.vm.define "server" do |serveurweb|
    serveurweb.vm.box = "ubuntu/trusty64"

    serveurweb.vm.box_check_update = false

    serveurweb.vm.network "forwarded_port", guest: 8080, host: 8082

    serveurweb.vm.network "private_network", type: "static", ip: "192.168.33.10"

    serveurweb.vm.synced_folder "./tomcatwebapps", "/opt/tomcat/webapps"

    serveurweb.vm.provider "virtualbox" do |vb|
      vb.gui = true
      vb.name = "serveurweb-tomcat"
      vb.memory = "1024"
    end
  end
end
