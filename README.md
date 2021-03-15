Role Name
=========

Role install and configure a host to be used as a golden image for etcd.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
        - role: centos8
        - role: etcd
          krole: "etcd"
          version: "v3.4.0"
          port: "2380"
          client_port: "2379"
          cert: "etcd.pem"
          key: "etcd-key.pem"
          ca_cert: "ca.pem"
          boot_wait_device: "sys-subsystem-net-devices-eth1.device"
          short_hostname: "etcd"
          domain: ""
          ip:
            - "10.1.0.11"
            - "10.1.0.12"
            - "10.1.0.13"

License
-------

BSD

Author Information
------------------

[Luis Gomes](https://github.com/luishmg/luishmg.github.io)
