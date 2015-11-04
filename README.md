# aws-utilities

Various utility processes that run on AWS and Ansible files to set them up

Assuming Ansible AWS dynamic inventory is set up and you have the
right Ansible Vault password for decrypting secrets in
`~/.vault_pass.txt`, start an AWS EC2 instance with a `Name` tag of
`utility-ec2-instance` and set up with:

```
ansible-playbook --private-key ~/.ssh/cadasta-utility.pem --vault-password-file ~/.vault_pass.txt site.yml
```
