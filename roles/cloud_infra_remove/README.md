cloud_server_remove
=========

Manage deployment of cloud servers

Requirements
------------

Collection openstack.cloud

Role Variables
--------------

instances: List of dictionaries
  - name: Server name
      cloud: Cloud for server to be built
      server_state: Whether server should be present or absent.  Default absent
      keypair: Ssh keypair for server
      flavor: Flavor of the server 
      security_groups: Security groups for server
      network: Network of server
      metadata: Dictionary of metadata for server
        AnsibleGroup: Ansible group for server

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: cloud_server_deploy
               cloud: "Example_cloud"
               name: "Servername"
               image: "boot_image_name"
               key_name: "ssh_key"
               flavor: "OS_Flavor"
               security_groups: "Security_group"
               network: "Network_name"
               metadata:
                 AnsibleGroup: host_group
           }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
