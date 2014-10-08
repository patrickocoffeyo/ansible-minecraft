#Ansible Minecraft

This Ansible playbook creates a basic Minecraft server on a vanilla ubuntu installation.

#Installation
1. Create a server running Ubuntu 14.04
2. Clone this repository ```git clone https://github.com/patrickocoffeyo/ansible-minecraft.git```
3. Open your Ansible hosts file, and a host record called ```minecraft_server```. Add your server's IP address to the host as an alias like so:
```bash
[minecraft_server]
alias ansible_ssh_host=XXX.XXX.XX.XX
```
4. Ensure that the system you'll be running Ansible can log into your server with the root user without a password (using SSH keys).
5. Run the playbook: ```ansible-playbook ansible-minecraft.yml```
6. Configure minecraft to your hearts desire :)