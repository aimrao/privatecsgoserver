# Installing and Configuring CSGO Server

## Installing
1. SSH to your AWS/GCP or any cloud machine running Ubuntu 16.04 (or greater) or Debain 9 (or greater) and run the following commands in order.
2. ```sudo dpkg --add-architecture i386; sudo apt update; sudo apt install curl wget file tar bzip2 gzip unzip bsdmainutils python util-linux ca-certificates binutils bc jq tmux netcat lib32gcc1 lib32stdc++6 libsdl2-2.0-0:i386 steamcmd ``` for Ubuntu.
3. ``` sudo dpkg --add-architecture i386; sudo apt update; sudo apt install curl wget file tar bzip2 gzip unzip bsdmainutils python util-linux ca-certificates binutils bc jq tmux netcat lib32gcc1 lib32stdc++6 ``` for Debian.
4. ``` adduser csgoserver ```
5. ``` su - csgoserver ```
6. ``` wget -O linuxgsm.sh https://linuxgsm.sh && chmod +x linuxgsm.sh && bash linuxgsm.sh csgoserver ```
7. ``` ./csgoserver install ```
8. CSGO server would start installing now and during installation it would ask for you GSLT token, which you can create by going [here](https://steamcommunity.com/dev/managegameservers).
9. After the installation is finished, copy the ```lgsm/config-lgsm/csgoserver/csgoserver.cfg``` to your server's ```lgsm/config-lgsm/csgoserver/``` directory and ``` serverfiles/csgo/cfg/csgoserver.cfg ``` to your server's ```serverfiles/csgo/cfg/``` directory. 
10. Add your GSLT token to ```lgsm/config-lgsm/csgoserver/csgoserver.cfg```. 
11. You can further configure your server like servername, admin password, game mode, etc. by making changes to the 2 config files mentioned above.
12. You can start your server using ``` ./csgoserver start ```, ``` ./csgoserver stop ``` to stop and ``` ./csgoserver restart ``` to restart.
13. More commands could be found by typing ``` ./csgoserver ```


Commands to host your own csgo server on any cloud platform like aws, gcp, etc.
