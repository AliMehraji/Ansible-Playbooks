Example Playbook
----------------

This is how you need to use playbooks but you may need comment some roles and use tags.

```
ansible-playbook playbooks/main.yml --tags "create_user"
```

Like Below For Role when you need user handling role in `playbooks/main.yml`

```
roles:
  - Update
  - Install-Python
  - User_Handling
  # - Docker
  # - Gitlab_runner
```
