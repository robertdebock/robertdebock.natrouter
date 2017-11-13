Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

public_interface - The interface to go out over, defaults to eth0
private_network - The CIDR notation of the network where traffic will come from, default to 192.168.1.0/24

Dependencies
------------

- robertdebock.bootstrap

Example Playbook
----------------

```
- hosts: servers
  roles:
    - role: robertdebock.natrouter
      public_interface: enp0s3
      private_network: 172.16.0.0/24
```

License
-------

Apache License, Version 2.0

Author Information
------------------

Robert de Bock <robert@meinit.nl>
