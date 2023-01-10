# Script to install and configure OpenVPN and Apache web-server

This script automatically install and configure OpenVPN on protocol UDP port 1194 and then install and reconfigure Apache web-server to give a opportunity to download client file without going to the server


Requirements:
- AWS free trial account 
- to have approximately 2 minutes ( to create instance )))

Steps:
- First you have to create you instance ( I used ec2 ubuntu-22.04 )
- Set up firewall settings: 
    - allow http traffic: TCP - 80
    - allow openvpn traffic: UDP - 1194
    - allow ssh traffic: TCP - 22 (optional) 
- Insert [script-openvpn-apache.sh](https://github.com/rlnq/tstopvnp/blob/main/script-openvpn-apache.sh) in user data

Pls qait a couple of minutes and download you file configuration 

