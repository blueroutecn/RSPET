# reverse_shell
A reverse shell 

DISCLAIMER: I really shouldn't have to say this but DON'T USE THIS WITHOUT THE COMPUTER OWNER'S CONSENT

Features:

-Reverse TCP/IP connection, circumventing victim-side firewall roules (in most cases) and NAT limitations.

-Trafic Masking. All traffic is sent XORed and not in clear text. For better masking swap port to 443.[1]

-Support for multiple connections. The Server part is built with support for multiple simulatneus connections, with Hosts list managment.

-Client script is tested and is compatible with PyInstaller (can be made into .exe).[2]

Deployment:

-The server is situated at the attacker's machine and running to accept connections

-The client is situated in the infected machine(s) and will initiate the connection and wait for input.

Execution:

In their current stated the scripts are executed as follows

-Server: python rev_shell_server.py (max_connections) 
max_connections defaults to 5 if left blank

-Client: python rev_shell_client.py (server_ip)

Many changes can be made to fit individual needs.

As always if you have any suggestion, bug report or complain feel free to contact me.

*[1]The idea for XORing as well as the skeleton for the client came from (http://www.primalsecurity.net) so if you like this pack of scripts you'll probably love what they do

*[2]Again check primalsecurity.net's perfect blogpost about producing an .exe
