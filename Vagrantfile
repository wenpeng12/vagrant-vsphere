# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. 
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  
		config.vm.box = 'dummy'
		config.vm.box_url = './example_box/dummy.box'  
		
		config.vm.hostname = ENV['host']
		
  

  config.vm.provider :vsphere do |vsphere|
    vsphere.host = '49.21.15.148'
    vsphere.resource_pool_name = 'Build'
    vsphere.template_name = 'clone2'
    vsphere.clone_from_vm = true
    vsphere.name = 'clone1'
    vsphere.user = 'root'
    vsphere.password = 'vagrant'
    vsphere.insecure = true
  end
end
