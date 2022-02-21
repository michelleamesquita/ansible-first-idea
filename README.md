# ansible-first-idea
Initiative to create my first playbook

How to run:

1) Create a file with secret, using `ansible-vault create secret`. It will ask for ansible_sudo_pass: mysudopassword 
2) Create a file vault.txt to remember the password that you gonna use to decrypt this secret file
3)RUN:
`ansible-playbook playbook-docker.yml -i inventory.txt --vault-password-file=vault.txt`

To use this idea:
Remember to create 2 VMs
1- ansible controller
sudo yum install ansible

2- ansible target
to set what you need with ansible


To change host:
sudo vi /etc/hostname
sudo vi /etc/hosts
shutdown now -r
