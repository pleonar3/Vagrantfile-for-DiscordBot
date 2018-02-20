Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.provision "shell", inline: <<-SHELL
    apt-get -y update
    apt-get -y install vim
    apt-get -y install git
    printf "set nocompatible\nset number\nsyntax on\nset tabstop=2\nset shiftwidth=2\nset expandtab" > ~/.vimrc     
    curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
    apt-get install -y nodejs
    npm install discord.js
    npm install string-tokenizer
    npm install mathjs
    npm install sqlite3
  SHELL
end
