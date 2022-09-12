
## extentions 

 Mate Translate 
 
 transover
 
 Adblock Plus
 
 Youtube Subtitle Downloader
 
 Bitwarden
 
 Grammarly 
 
 Wappalyzer == WhatRuns
 
 Web Developer

### Necessary apps
```
sudo apt install axel
```
usage: axel -ac -o[name] -s[speed] 

```
sudo apt install vlc
```
vlc subtitle word search 
https://github.com/tcrespog/vlc-subtitle-word-search

```
sudo snap install --classic code
```
```
sudo apt install unrar
```
```
sudo apt install python3
```
```
sudo apt install python3-pip
```


### installing chrome
```
sudo dpkg -i google-chrome-stable_current_amd64.deb 
```
 


### installing cisco

```
sudo apt install network-manager-openconnect-gnome
```

 guaidance:
        http://sspeedvpn12.xyz/cisco-for-linuxe/
	
 addreses:
        http://sspeedvpn12.xyz/servernew/index.php



### installing guake f12
```
sudo apt install guake
```

 guake add to startup
 
recommanded changing
 scrolling --> infinite scrolling
 main bar --> hide on lose focus
          --> geomtry --> on your taste


             
### installing telegram
  https://desktop.telegram.org/
or
```
wget -O- https://telegram.org/dl/desktop/linux | sudo tar xJ -C /opt/
```
```
sudo ln -s /opt/Telegram/Telegram /usr/local/bin/telegram-desktop
```
or
```
sudo snap install telegram-desktop
```
cli
```
sudo snap install telegram-cli
```


### instaling oh my zsh
  guaidanc:https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH
  added plugins /installation/zshrc

```
sudo apt install zsh
```
```
chsh -s $(which zsh)
```
```
sudo apt install curl
```
```
sudo apt install git
```
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```
```
nano .zshrc
```
  ZSHـTheme="" 
  thems:https://github.com/robbyrussell/oh-my-zsh/wiki/Themes
  
```
source .zshrc
```

  reastart
 

### installing zsh plugins(autosuggestions)

  guaidenc:https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md
```  
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions 
```
```
nano .zshrc
```
  plugins=(sudo extract git zsh-autosuggestions)
  
```
source .zshrc
```

### installing trash box:

```
sudo apt install npm
```
```
sudo npm install --global trash-cli
```
trash "at"
 
--4more u can change rm command
```
nano .zshrc
```

  add :
       alias rm=trash



### installing pycharm
```
sudo snap install pycharm-professional --classic
```

-ssh key for git
```
cd .ssh
```
```
ssh-keygen
```
```
cat {{cat /home/scarf/.ssh/id_rsa.pub}}
```
```
git--> settin-->ssh
```



### installing anaconda
  https://www.anaconda.com/distribution/#download-section
  Anaconda3-2019.10-Linux-x86_64.sh
  bash . sh

  in zshrc:
  add export PATH="/home/username/miniconda/bin:$PATH"



### installing docker
```
sudo apt install apt-transport-https ca-certificates curl software-properties-common
```
```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
```
```
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"
```
```
sudo apt update
```
```
apt-cache policy docker-ce
```
```
sudo apt install docker-ce
```
```
sudo systemctl status docker
```
 guaidanc:
 https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-18-04



### installing docker-compose
```
sudo curl -L "https://github.com/docker/compose/releases/download/1.27.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```
```
sudo chmod +x /usr/local/bin/docker-compose
```
```
sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
```
 guaidanc:
 https://docs.docker.com/compose/install/
 
 
### installing docker postgresql
```
docker pull postgres
```
```
docker run --name postgresql-container -p 5432:5432 -e POSTGRES_PASSWORD=somePassword -d postgres
```
```
docker ps -a
```
```
docker exec -it <PSQL-Container-ID> bash
```

pycog2 connecting:
https://stackoverflow.com/questions/48522640/failure-to-connect-to-docker-postgresql-instance-from-python



### installing local postgressql (not recommanded because of authentication problems)
 sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list'
 wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -
 sudo apt-get update
 sudo apt-get install postgresql
 guaidanc:
 https://www.postgresqltutorial.com/install-postgresql-linux/
 
 solving_authentication_problem
 https://stackoverflow.com/questions/1471571/how-to-configure-postgresql-for-the-first-time
 https://stackoverflow.com/questions/42653690/psql-could-not-connect-to-server-no-such-file-or-directory-5432-error
 


-installing uget
 official
 https://github.com/ugetdm/uget-integrator/wiki/Installation
 ```
 sudo add-apt-repository ppa:uget-team/ppa
 ```
 ```
 sudo apt update
 ```
 ```
 sudo apt install uget-integrator
 ```
  
 unofficial
 https://tipsonubuntu.com/2016/07/12/latest-uget-ubuntu-16-04/
 sudo add-apt-repository ppa:plushuang-tw/uget-stable
 sudo apt update
 sudo apt install uget



### installing postman
```
wget https://dl.pstmn.io/download/latest/linux64 -O postman-linux-x64.tar.gz
```
```
sudo tar -xvzf postman-linux-x64.tar.gz -C /opt
```
```
sudo ln -s /opt/Postman/Postman /usr/bin/postman
```
```
cat << EOF > ~/.local/share/applications/postman2.desktop
[Desktop Entry]
Name=Postman
GenericName=API Client
X-GNOME-FullName=Postman API Client
Comment=Make and view REST API calls and responses
Keywords=api;
Exec=/opt/Postman/Postman
Terminal=false
Type=Application
Icon=/opt/Postman/app/resources/app/assets/icon.png
Categories=Development;Utilities;
EOF
```
 
 guaidance:
	https://linux4one.com/how-to-install-postman-in-linux/#Install_Postman_in_Linux



### installing AnyDesk
```
wget -qO - https://keys.anydesk.com/repos/DEB-GPG-KEY | sudo apt-key add -
```
```
echo "deb http://deb.anydesk.com/ all main" | sudo tee /etc/apt/sources.list.d/anydesk-stable.list
```
```
sudo apt update
```
```
sudo apt install anydesk
```



### installing vmvare
https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html
```
sudo apt-get update 
```
```
sudo apt install gcc build-essential 
```
```
chmod +x [name of downloaded file VMware-Player-16.0.0-16894299.x86_64.bundle]
```
```
sudo ./[name of downloaded file VMware-Player-16.0.0-16894299.x86_64.bundle]
```
restart + del in cpu turn on vm engine

installing packages needed
https://communities.vmware.com/t5/VMware-Workstation-Pro/VMWare-Workstation-fails-to-compile-modules-on-Fedora-31/m-p/1871268
install 
wget https://github.com/mkubecek/vmware-host-modules/archive/workstation-15.5.1.tar.gz
in ectracted folder 
make 
sudo make install

guaidabce:
https://www.youtube.com/watch?v=OHEiP1V0cCI



### installing avidemux
```
sudo add-apt-repository ppa:ubuntuhandbook1/avidemux
```
```
sudo apt update
```
```
sudo apt install avidemux2.7-qt5 avidemux2.7-qt5-data avidemux2.7-plugins-qt5 avidemux2.7-jobs-qt5
```
 Uninstall:
  sudo apt remove --autoremove avidemux2.7-*






## mint

-installing redshift 2 qredshift in mint
```
sudo apt-get install redshift
```
download 
https://cinnamon-spices.linuxmint.com/files/applets/qredshift@quintao.zip
extract
Enable qredshift in the applet 
sudo apt-get remove redshift-gtk

guaidence:
https://cinnamon-spices.linuxmint.com/applets/view/313



### installing snap on mint
```
sudo rm /etc/apt/preferences.d/nosnap.pref
```
```
sudo apt install snapd
```
```
sudo apt update
```







-- all

### make sudo for all docker
```
sudo usermod -a -G docker $USER
```

### Britghtness:
```
xrandr | grep " connected" | cut -f1 -d " "
```
```
LVDS-1
```
```
xrandr --output [monitor-name] --brightness [brightness-level]
```
```
xrandr --output LVDS-1 --brightness 0.75
```

#### ubuntu hide topbar
https://ubuntuhandbook.org/index.php/2020/08/top-panel-auto-hide-ubuntu-20-04/
```
sudo apt install gnome-shell-extension-autohidetopbar
```
Alt+F2
r
Extensions
“Hide Top Bar” 

### grub-customizer
```
sudo add-apt-repository ppa:danielrichter2007/grub-customizer
```
```
sudo apt update
```
```
sudo apt-get install grub-customizer
```

#### open with gedit
```
sudo -H gedit {file}
```

#### make default new format
```
cd ~/Templates 
```
```
sudo touch mypy.py
```

#### see config
```
inxi -Fxzd
```

-file Permission
https://www.guru99.com/file-permissions.html

-linux change password
https://www.youtube.com/watch?v=Nnxj7osSjNU&feature=youtu.be

#### delet keyring
```
rm -rf ~/.local/share/keyrings
```

#### delete kernel
```
sudo apt remove linux-image-5.11.0-22-generic linux-headers-5.11.0-22-generic
```
```
sudo apt remove --purge linux-image-5.11.0-22-generic linux-headers-5.11.0-22-generic
```
```
sudo rm -rf /usr/lib/modules/5.11.0-22-generic
```
```
sudo apt install --reinstall linux-image-5.11.0-22-generic
```
