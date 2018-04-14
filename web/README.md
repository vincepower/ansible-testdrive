# Installs Apache HTTPD
----------------

Uses the hosts in the [web] section in /etc/ansible/hosts for the server.

Variables are set in the role, the only exposed one is the default port.
```
nano web/roles/httpd/vars/main.yml
```

Run the installation using the follow command:
```
ansible-playbook install-httpd-php.yml
```

