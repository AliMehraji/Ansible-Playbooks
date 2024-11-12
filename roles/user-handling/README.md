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
USER_NAME:         # New Username will be created or a user will be deleted or update password 
USER_PASSWORD:     # New Username's Password
USER_SHELL:        # New Username Shell can be /bon/bash or /bin/sh
COMMENT:           # A Brief Comment for newuser
NEW_PASSWORD:      # This is gonna be used in updating password task for a user who has forgot , you need to specify username in USER_NAME to update password.
```

Example Playbook
----------------

This is how you need to use playbooks but you may need comment some roles and some tasks when you use .

```bash
ansible-playbook playbooks/main.yml --tags "create_user"
```

```yaml
roles:
    - Docker
    - gitlab-runner
    - User-Handling
```

```yaml
- include_tasks: Create-User.yml
- include_tasks: Update-Password.yml
- include_tasks: Delete-User.yml
```

License
-------

Buy Me A Beer ;\)

Author Information
------------------

Name : Ali Mehraji </br>
Email: a.mehraji75@gmail.com