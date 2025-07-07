# all-about-ansible
this repo refers to ansible knowledge
-----------------------------
Author : Saikrishna

Date : July 2025

Topic : Ansible
-----------------------------

1. Ansible is powerful tool and widely used as Configuration management tool.

2. Written in Python Language, so python is the pre-requisite for installing Ansible.

3. Agentless Architecture which means ansible is not needed to be installed in every target node.

4. Passwordless Authentication which Connects with Linux through "SSH" and Windows through "winrm", which is also pre-requisite.

5. Simple YAML language unlike the other tools like puppet and chef which are complex languages.

6. Controlled Node and Managed Nodes Architecture.

7. Uses Push mechanism on to the target servers. 

8. Most widely Used in Network Automation.

9. Eliminate repitition which automates.

10. Manage and maintain system configurations.

11. Perform zero-downtime rolling updates.

12. Idempotence.
----------------------------------------------------------------------------------------

                         Commands
                        ----------

>> brew/yum/apt install ansible (Installing Ansible in MacOS, RHEL and Ubuntu)

>> pip install ansiblev (Installing Ansible using python package manager)

>> ansible --version. 

>> ansible -i inventory all -m "shell" -a "df -h & touch file & nproc".

>> ansible-playbook -i inventory <playbook.yml>

>> ansible-playbook -i inventory <playbook.yml> --check 

>> ansible-playbook -i inventory <playbook.yml> -vvv 

>> ansible-galaxy role init <role-name>

-----------------------------------------------------------------------------------------

Passwordless Authentication

>> ssh-copy-id -f "-o IdentityFile <PATH TO PEM FILE>" ubuntu@<INSTANCE-PUBLIC-IP>

>> Copy the public key of controlled node to the target nodes in the ~/.ssh/authorised_keys file.

>> Can also setup Password Authentication in the target nodes with setting the values "yes"
 

Inventory File

>> 

Ansible-Role Hierarchy Structure



