# Installs phpMyAdmin
----------------

Uses the hosts in the [web] section in /etc/ansible/hosts for the server.

Variables are set in the playbook.

Yes, there is an easier way to install phpMyAdmin with yum, but this shows that Ansible can download and work with files. It also configures the phpMyAdmin instance server to update its default localhost to point at the database server.

Run the installation using the follow command:
```
ansible-playbook install-phpmyadmin.yml
```

