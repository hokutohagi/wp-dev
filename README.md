## WordPress+Nginx+PHP-FPM Deployment

### ホストOS動作環境
  VirtualBox 5.0
  Vagrant 1.8.1

### ゲストOS動作環境
  Cent0S 6.7
  Ansible 1.9.4
	wp_version 4.2.4

### vagrantの実行は以下の様に行う:
  git clone git@github.com:de2p-shikataro/wordpress-development.git
	cd wordpress-development
	vagrant up

### WordPressへのアクセスは以下のURLへ
http://192.168.33.10/wp-admin/install.php
