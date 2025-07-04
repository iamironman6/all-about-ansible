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

4. Connects Linux through "SSH" and Windows through "winrm".

5. Simple YAML language unlike the other tools like puppet and chef which are complex languages.

6. Controlled Node and Managed Nodes Architecture.

7. Uses Push mechanism on to the managed servers. 

8. Most widely Used in Network Automations also.

9. Eliminate repitition.

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

Ansible-Role Hierarchy Structure
--------------------------------



