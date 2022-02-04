configure_firewall
=========

Installs and configures firewalld

Requirements
------------

N/A

Role Variables
--------------

firewall_services:  Services to be enabled through firewall
firewall_tcp_ports: TCP ports to be enabled through firewall
firewall_udp_ports: UDP ports to be enabled through firewall

Dependencies
------------

N/A

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: configure_firewall
             vars:
               firewall_services:
                 - http
           }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
