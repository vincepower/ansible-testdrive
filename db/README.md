# Installs MariaDB
----------------

Uses the hosts in the [db] section in /etc/ansible/hosts for the server.

Uses all hosts for the client.

You can edit the default variables are set in the mariadb role including username, password, and port.
```
nano roles/mariadb/vars/main.yml
```

Run the installation:
```
ansible-playbook install-mariadb.yml
```

