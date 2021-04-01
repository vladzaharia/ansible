Ansible Role: AptProxy
=========

Configure Apt to use a proxy of your choice. I'm creating this role for learning and experimentation. Feel free to make suggestions, issues, or submit pull requests.

Requirements
------------

You should have an Apt proxy setup somewhere such as apt-cacher-ng. If you use this role w/o specifying a valid proxy Apt will fail!

Role Variables
--------------

Variables you can set are listed below with default variables (see `defaults/main.yml`);

    apt_proxy_protocol: "https"

The protocol to use to connect to the proxy.

    apt_proxy_url: "localhost:3142"

The URL to connect to.

Dependencies
------------

This role has no other dependencies.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: sitedyno.apt_proxy }

License
-------

BSD

Author Information
------------------

Copyright 2016 Heath Nail (sitedyno)
