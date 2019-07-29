# check_udp_port
Simple shell script that uses nmap utility to check if a remote host is listening on a UDP port and what that service is.
For Debian 10 and LibreNMS

## Usage
´check_udp_port: -H remote_host -p port -s service_name´

-H Name or IP of remote host

-p UDP port number to check

-s Name of the service that should be listening on the port


Critical: if service is 'unknown' or state is not open

Warning: if service name expected does not match service name listening on the port

OK: if the port is open and service name expected matches service name listening.

## Based on 
https://exchange.nagios.org/directory/Plugins/Network-Protocols/*-TCP-and-UDP-(Generic)/check_udp_port/details
