# Script to install and configure OpenVPN and Apache web server

This script automatically installs and configures OpenVPN on UDP port 1194, then installs and reconfigures the Apache web server to allow client file uploads without going to the server


Requirements:
- Free AWS trial account
- about 2 minutes (to create an instance)))

Steps:
- First you have to create you instance ( I used ec2 ubuntu-22.04 )
- Set up firewall settings: 
    - allow http traffic: TCP - 80
    - allow openvpn traffic: UDP - 1194
    - allow ssh traffic: TCP - 22 (optional) 
- Insert [script-openvpn-apache.sh](https://github.com/rlnq/tstopvnp/blob/main/script-openvpn-apache.sh) in user data

Wait a few minutes and download the client file at: *http://*your_public_ip*/config*

