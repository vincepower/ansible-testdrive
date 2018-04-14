# Installs nginx and PHP
----------------

Uses the hosts in the [web] section in /etc/ansible/hosts for the server.

Variables are set in the role, the only exposed one is the default port.
```
nano web/roles/nginx/vars/main.yml
```

Run the installation using the follow command:
```
ansible-playbook install-nginx-php.yml
```

