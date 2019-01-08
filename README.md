Role Name
=========

Install Red Hat Satellite Beta 6.4 

Requirements
------------

for the instalation the system requires:

4-core 2.0 GHz CPU at a minimum
A minimum of 20 GB memory is required for the Satellite Server to function
8Gb of memory ram as minimum
8Gb of swap
***important***
Ensure that storage is available on the /var file system to prevent storage problems

Role Variables
--------------
please provide this variables in your inventory

[satellite]
</br>
192.168.4.16

[satellite:vars]
satellite_initial_organization= "initial-organization"
satellite_initial_location= "initial-location"
satellite_username= "the-admin-user"
satellite_password= "the-password-of-the-admin-page"
satellite_dhcp_managed= false
satellite_dns_managed= false


this role install satellite acording of the basic instalation

To view all of the configurable options, enter the satellite-installer --scenario
satellite --help command

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------
one you provide the vars in your inventory, run the runsetup.yml the role will ask you for rhn user & password

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
