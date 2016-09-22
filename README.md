ansible-role-teamcity
=========

This role Installs and updates TeamCity server from JetBrains

Requirements
------------

Only works on debian systems so far

Role Variables
-------------
``` yaml
teamcity_version: "10.0.2"
download_directory: "/tmp/"
teamcity_install_folder: "/opt/TeamCity"
teamcity_data_path: "{{teamcity_install_folder}}/data"
teamcity_user: "teamcity"
teamcity_group: "teamcity"
teamcity_http_port: "80"
initSystem: "system.d"

```

Dependencies
------------



Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```
   - hosts: teamcity
     roles:
     - role: ansible-role-teamcity
       teamcity_http_port: 8080
```
License
-------

BSD

Author Information
------------------

[merodwin](https://github.com/merodwin)
