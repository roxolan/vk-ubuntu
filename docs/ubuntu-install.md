### Install VMWare tools

https://kb.vmware.com/s/article/1022525

`$ sudo ./vmware-install.pl`

without -d: asks a lot of questions on (default) location of the folders

### sudo access

`$ sudo visudo`

add NOPASSWD:ALL to %sudo

### hostname
`$ sudo gedit -> /etc/hostname, /etc/hosts`

http://ubuntuhandbook.org/index.php/2014/04/change-hostname-ubuntu1404/


### install Emacs->Spacemacs
`$ sudo apt update`

`$ sudo apt upgrade`

`$ sudo apt install emacs`

`$ git clone https://github.com/syl20bnr/spacemacs ~/.emacs.d`

### Install Docker
https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/#install-docker-ce
- while not available for u17.10: https://gist.github.com/levsthings/0a49bfe20b25eeadd61ff0e204f50088

- ... `$ sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu zesty stable"`

### Install docker-compose
`sudo curl -L https://github.com/docker/compose/releases/download/1.18.0-rc2/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose`

`sudo chmod +x /usr/local/bin/docker-compose`


### Add accesss key to bitbucket to seamlessly commit

https://confluence.atlassian.com/bitbucket/use-access-keys-294486051.html

`$ ssh-keygen`

-> bitbucket >

### Install Chrome
https://askubuntu.com/questions/510056/how-to-install-google-chrome

`$ wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add -`

`$ echo 'deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main' | sudo tee /etc/apt/sources.list.d/google-chrome.list`

`$ sudo apt update`

`$ sudo apt install google-chrome-stable`

### Install WebStorm
https://www.jetbrains.com/webstorm/download/
- font in WS terminal console: Settings > Editor > Color Scheme > Console Font
- -> install plugin: Markdown Navigator

### Install roboto and firacode fonts
`sudo apt install fonts-roboto`
- -> set 'Overeride default fonts by' roboto <12>
`sudo apt install fonts-firacode`

### Install nvm
https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-16-04

`$ sudo apt install build-essential libssl-dev`

`$ curl -sL https://raw.githubusercontent.com/creationix/nvm/v0.33.8/install.sh -o install_nvm.sh`

`$ bash install_nvm.sh`

`$ nvm ls-remote`

`$ nvm install 7.1.0`

`$ nvm alias default 7.1.0`

### Install zsh & oh-my-zsh
`$ sudo apt install zsh`

`$ zsh --version`

`$ echo $SHELL`

`$ chsh -s $(which zsh) vk`

`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`


