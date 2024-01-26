Example Playbook
----------------

This is how you need to use playbooks but you may need comment some roles and some tasks when you use .

```
ansible-playbook playbooks/main.yml 
```

Like Below For Role when you need user handling role in `playbooks/main.yml`

```
roles:
    #- Docker
    #- gitlab-runner
    - user-handling
```

And For Task if you dont want some task just comment them in `roles/role-name/tasks/main.yml` like below:</br>
If You just need to Delete a user do some comments in `roles/user-handling/tasks/main.yml`

```
# - include_tasks: Create-User.yml
# - include_tasks: Update-Password.yml
- include_tasks: Delete-User.yml
```
