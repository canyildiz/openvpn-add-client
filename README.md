# openvpn-add-client
A basic bash script to create client files on a openvpn server in a single line

## Usage
This is a very simple script I use on my debian jessie server running OpenVPN 2.4 on it. I place this file into `/etc/openvpn` directory and run it there in following format:

`./add-client <clientid>`

then it creates a single ovpn file with given clientid, containing necesarry certificates, located under `/etc/openvpn/easy-rsa/clients` folder.

## Prerequisites

This script assumes following environment is already running:
- Debian Jessi (not tested on other distro and/or versions, may also run on Ubuntu 16.04)
- OpenVPN 2.4 (not tested on other versions)
- Server config and certificates for OpenVPN already created (in most cases following files should exist:
  - server.conf, server.crt, server.key in `/etc/openvpn`
  - ca.crt in `/etc/openvpn/easy-rsa`
  - client.ovpn (generic config without certificates) in `/etc/openvpn/easy-rsa/keys/`

## Future
This is very beginning of this script. I will improve the script and this README soon (I hope :-))
