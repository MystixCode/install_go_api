# install_go_api
Script to install following on a debian10 server:
- sudo
- nginx + certbot
- firewall
- fail2ban
- git
- golang
- postgresql
- mariadb
- go api ([go-rest-api](https://github.com/gabrielix29/go-rest-api)/[nyx](https://github.com/authenter/nyx))

still unstable dev version!

### HowTo
- create a debian10 system with ssh and standard systemtools
- get a domain name and create dns record to your WAN IP
  - [empty]  ->  WAN IP
  - www      ->  WAN IP
  - api      ->  WAN IP
  
- on your router: create port forwarding for http and https to your debian10 system 
- copy this bash script to your debian10 system and execute it as normal user
- you will have to fully disconnect,reconnect and restart the script after sudo installation and after golang installation. You will be warned with orange text warning


### TODO
- GOPATH in .profile doesnt work anymore
- testing, fixing, errorhandling
- make it not necessary to disconnect and restart script after sudo and golang installation maybe with source command
