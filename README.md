Role Name
=========

This role installs WP-CLI (the WordPress CLI tool) on a given Ubuntu 18.04 server.

Support for more versions and operating systems will be added as soon as I can test the same.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

Variable | Type | Default | Usage
--- | --- | --- | ---
`wp_cli_install_location` | string | `/usr/local/bin` | Folder to install wp-cli to
`wp_cli_phar_url` | string | See defaults | Source URL for wp-cli phar
`wp_cli_force_replacement` | boolean | no | Whether to force replacement of existing file

Dependencies
------------

None

Example Playbook
----------------

```
    - hosts: servers
      roles:
         - { role: vidur.wp-cli, wp_cli_install_location: /usr/bin }
```

License
-------

MIT

Author Information
------------------

Vidur Butalia