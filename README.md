Ansible Role: NFS Server 
=========

This role install NFS server

Requirements
------------
None

Role Variables
--------------

| Name                      | Default value                         |        Requird       | Description                                                                 |
|---------------------------|---------------------------------------|----------------------|-----------------------------------------------------------------------------|
| nfs_mount_point           | /exports                              |         no           | Export directory where will be mounted                                      |
| nfs_block_dev_name        | /dev/sdc                              |         no           | Block device name                                                           |

Dependencies
------------

None



Example Playbook
----------------
~~~
- name: Example Playbook
  hosts: localhost
  gather_facts: false

  roles:
    - { role: Jooho.nfs-server }
~~~

Information
----------
- The block device will be formatted for LVM


License
-------

BSD/MIT

Author Information
------------------

This role was created in 2018 by [Jooho Lee](http://github.com/jooho).

