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
   (ssh-copy-id -f "-o IdentityFile key-pair.pem" ubuntu@54.91.86.193)

>> Copy the public key of controlled node to the target nodes in the ~/.ssh/authorised_keys file.

>> Can also setup Password Authentication in the target nodes with setting the values "yes"
 

Inventory File

>> It has IP addresses of managed nodes and we can group the managed nodes into multiple. 


Ansible-Vault

1. Create a password for vault
    
   > openssl rand -base64 2048 > vault.pass
   
2. Add your AWS credentials using the below vault command
    
   > ansible-vault create/encrypt/derypt group_vars/all/pass.yml --vault-password-file vault.pass

Ansible-Role Hierarchy Structure

>> 

Ansible-Demo
---------------
Task 1:
Create three(3) EC2 instances on AWS using Ansible loops

2 Instances with Ubuntu Distribution
1 Instance with Redhat Distribution
Hint: Use <connection: local> on Ansible Control node.

Task 2:
Set up passwordless authentication between Ansible control node and newly created instances.

Task 3:
Automate the shutdown of Ubuntu Instances only using Ansible Conditionals

Hint: Use when condition on ansible gather_facts
 
-------------------------------------------------