# Auto_EAP

## Introduction
-----
Auto_EAP.py is a script designed to perform automated brute-force authentication attacks against various types of EAP networks. Using the python library wpaspy, created by Jouni Malinen <j@w1.fi> 
to interact with the wpa_supplicant damon, automated authentication attacks can be preformed with the intent of not causing account lock-outs.

## Installation
-----

Run `RunMeFirst.py` within the root directory of Auto_EAP. This will compile the wpaspy library as well as setup a stand alone wpa_supplicant.conf file that Auto_EAP.py will use for testing, leaving the system’s wpa_supplicant config file untouched.  

## Help
-----

'./Auto_EAP.py -h'
'usage: Auto_EAP.py [-h] -i Interface -s SSID -U Usernamefile -p Password -K'
                   Key_mgmt -E Eap_type

optional arguments:
  -h, --help            show this help message and exit
  -i Interface, --interface Interface
                        The Interface to use
  -s SSID, --ssid SSID  The SSID to attack
  -U Usernamefile, --User Usernamefile
                        Path to username file
  -p Password, --password Password
                        Password to use
  -K Key_mgmt, --key_mgmt Key_mgmt
                        Key_Management type to use
  -E Eap_type, --eap_type Eap_type
                        Eap type to use'


## Todo list
-----
[-] Add multi-threading functionality
[-] Add support for password lists

