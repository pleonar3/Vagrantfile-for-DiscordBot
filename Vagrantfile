Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.provision "shell", inline: <<-SHELL
    apt-get -y update
    apt-get -y install vim
    apt-get -y install git
    printf "set nocompatible\nset number\nsyntax on\nset tabstop=2\nset shiftwidth=2\nset expandtab" > ~/.vimrc     
    #nodejs and npm
    apt-get -y install nodejs
    apt-get -y install npm
    #nodejs packages
    npm install --save discord.js
    npm install node-tokenizer
    npm install mathjs
    npm install node-json-db 
  SHELL
end
