realloc.tini
=========

Ensures tini init is installed. Usefull for building Docker images with Ansible.

Role Variables
--------------

Version of tini to be installed. See [list of releases](https://github.com/krallin/tini/releases) on GitHub.

```yaml
tini_version: v0.9.0
```

Path to install tini binary.

```yaml
tini_path: /sbin/tini
```

Maybe you want to disable certificates validation to allow MITM proxy.

```yaml
tini_validate_certs: yes
```

Example Playbook
----------------

```yaml

    - hosts: servers
      roles:
         - role: realloc.tini
```

License
-------

GPLv3

Author Information
------------------

Stanislav Bogatyrev <realloc@realloc.spb.ru>
