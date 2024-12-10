# How To

This is how you need to use playbooks but you may need comment some roles and use tags.

```bash
ansible-playbook playbooks/main.yml --tags "create_user"
```

## Playbooks Notes

For Docker Installation via `playbooks/docker.yml`:
> install the `geerlingguy.docker` role

```bash
proxychains4 ansible-galaxy role install -r requirements.yaml --roles-path ./roles
```
