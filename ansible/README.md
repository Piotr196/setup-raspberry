Before running playbook
```
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/rpi_final.pem
```
ansible-playbook -i switch_users_inventory.yml switch_users_playbook.yml --extra-vars "ansible_sudo_pass=yourPassword"