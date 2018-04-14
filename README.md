# Ansible Examples
----------------

This repository contains the samples included in Ansible Core (Engine) Test Drives I manage. They are really only tested on Ansible 2.4+ and RHEL 7.4+

## ansible-testdrive/common

To show what can be done in a playbook, this section uses a single playbook that to install latest updates, NTP, and enable firewalld on all servers.

```
cd /home/ansible/ansible-testdrive/common
ansible-playbook install-common.yml
```

## ansible-testdrive/db

To show you can do different things on different hosts within the same playbook, this contains a role that installs MariaDB and a role to include the client on all servers.

group_vars/all includes variables used for the base setup including MariaDB's root password

```
cd /home/ansible/ansible-testdrive/db
ansible-playbook install-mariadb.yml
```

Using the DbConsole address you can now connect and use any MySQL 5.6+ compatible client.

## ansible-testdrive/web

To show how roles can work, this uses two roles. One installs Apache HTTPD and the second installs PHP.

group_vars/all includes variables used for the base setup include port.

```
cd /home/ansible/ansible-testdrive/web
ansible-playbook install-httpd-php.yml
```

Using the WebConsole address you can now connect to http://$WebConsole/info.php

