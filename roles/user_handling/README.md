# User-Handling

Requirements
------------

Because of depricating python crypto library in python 13 version its better to install `passlib` instead.

```bash
pip3 install passlib
```


Role Variables
--------------

```
user_name:         # New Username will be created or a user will be deleted or update password 
user_password:     # New Username's Password
user_shell:        # New Username Shell can be /bon/bash or /bin/sh
user_ssh_key:      # Add Username SSH-Key 
user_comment:      # A Brief Comment for newuser
user_new_password: # updating user password
```

Example Playbook
----------------

This is how you need to use playbooks but you may need comment some roles and some tasks when you use .

```bash
ansible-playbook playbooks/main.yml --tags "create_user"
```

```yaml
  roles:
    - os_update
    - install_python
    - user_handling
    - install_docker
    - install_gitlab_runner
```

License
-------

Buy Me A Beer ;\)

Author Information
------------------

Name : Ali Mehraji </br>
Email: a.mehraji75@gmail.com