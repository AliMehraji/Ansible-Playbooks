# TODO

- [ ] First Write All Creation And Deletion
- [ ] 2nd Separate Parts for Terraform

- Consider the Postgresql Cluster Scenario
  - 3 Etcd Nodes
  - 3 Postgresql Nodes


- [ ] Create Folder (Do it by Terraform)
- [ ] Create VM (Template os and ssh hardened , deploy by terraform)
  - [ ] AutoStart (by Terraform)
  - [ ] CPU HotAdd (by Terraform)
    - [ ] CPU cores per Socket (by Terraform)
  - [ ] Memory HotAdd (by Terraform)
  - [ ] Network (by Terraform)
    - [ ] Which Network (by Terraform)
    - [ ] DHCP (by Terraform)

  - [ ] Add Disk (Either Ansible or **terraform**)
    - [ ] Define what to add like `/dev/sdc, /dev/sdd`
    - [ ] From which storage (vm1, vm2 , bk1 ,...)
    - [ ] Disk Policy

  - [ ] LVM Resize (Ansible)
    - [ ] Install the `parted` or use ansible module for gdisk to do the `gdisk /dev/sdx` (install in its dependencies)
    - [ ] Implement add another vg and lv (for Postgres use case) Ansible
    - [ ] Use Variable For lv, vg , device name , ...
    - [ ] `resize2fs`

- [ ] Delete VM (Terraform )

- [ ] Some Variables From inventory for vm_management
- [ ] Connection to vCenter Host User, Password from Ansible-Vault 
