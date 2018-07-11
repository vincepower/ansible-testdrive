# Ansible Examples
----------------

This repository contains the samples included in Ansible Core (Engine) Test Drives I manage. They are really only tested on Ansible 2.4+ and RHEL 7.4+

## ansible-testdrive/common

To show what can be done in a playbook, this section uses a single playbook that to install latest updates, NTP, and enable firewalld on all servers.

```
Instructions are in common/README.md
```

## ansible-testdrive/db

To show you can do different things on different hosts within the same playbook, this contains a role that installs MariaDB and a role to include the client on all servers.

Using the DbConsole address you can now connect and use any MySQL 5.6+ compatible client.

```
Instructions are in db/README.md
```

## ansible-testdrive/web

To show how roles can work, this uses two roles. One installs Apache HTTPD and the second installs PHP.

Using the WebConsole address you can now connect to http://$WebConsole/info.php

```
Instructions are in web/README.md
```

## ansible-testdrive/phpmyadmin

Downloads, installs, and configured phpMyAdmin on the web server to manage the database server.

Also configured the phpMyAdmin instances on the web server to point at the database server by default using text replacement as default is always to use localhost.

```
Instructions are in phpmyadmin/README.md
```

