#
# Get OS images from https://github.com/theprotos/env-generic.git
#

Vagrant.configure("2") do |config|

  config.vm.define "node1" do |node1|
    node1.vm.box = "linux-generic"
    node1.vm.hostname = "node1"
    node1.vm.network "private_network", ip: "192.168.200.200"
###  vagrant up; vagrant rsync-auto
#    node1.vm.synced_folder ".", "/vagrant",
#        type: "rsync",
#        rsync__auto: true,
#        rsync__exclude: ['Vagrantfile'],
#        rsync__args: ["-z"]
    node1.vm.synced_folder ".", "/vagrant", type: "virtualbox"
  end

end
