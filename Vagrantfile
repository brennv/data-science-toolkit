VAGRANTFILE_API_VERSION = "2"
Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.box = "datascienceinc/data-science-toolkit"

  config.vm.provider "virtualbox" do |v|
    v.memory = 4096
    v.cpus = 2
    v.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
    v.customize ["modifyvm", :id, "--natdnsproxy1", "on"]
  end

  unless Vagrant.has_plugin?('vagrant-hostsupdater')
    system('vagrant plugin install vagrant-hostsupdater') || exit!
    exit system('vagrant', *ARGV)
  end

  config.hostsupdater.remove_on_suspend = true

  config.vm.define "oss-data-science-toolkit" do |node|
      node.vm.synced_folder ".", "/vhd", type: "nfs"
      node.vm.network "private_network", ip: "192.168.32.4"
      node.vm.hostname = "datascience.dev"
  end

end
