# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure(2) do |config|

  # boxが存在しなければ新規にCenOS6.7のboxをダウンロード
  config.vm.box = "CentOS67"
  config.vm.box_url = "https://github.com/CommanderK5/packer-centos-template/releases/download/0.6.7/vagrant-centos-6.7.box"

  # ゲストOSのIPアドレスの設定
  config.vm.network "private_network", ip: "192.168.33.10"

  # ansibleの設定
  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "ansible/site.yml"
  end

end
