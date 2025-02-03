### Ansible Coding challenge ###

**Terraform**
# EC2 (VM) will be provisioned by terraform code

# Directory structure of Terraform code :-

├── terraform/

       ├── main.yml
       ├── output_variables.tf
       ├── project_variables.tf
       ├── statfile.tf

**Ansible**

# Configuration of EC2 (VM) with Ansible:

• Install the following software packages on the VM:

o nginx

o git

o python3


• Configure the nginx server:

o Default webpage should display: "Welcome to the DevOps Challenge".

• Ensure the following system settings:

o Disable root login via SSH.

o Set a specific SSH port (e.g., 22).

• Create a new system user devops:

o Add it to the sudo group.

o Set up an SSH key for the devops user.


#Directory structure of Ansible code :-

├── ansible/

       ├── ansible_playbook.yml
       ├── inventory.json
       ├── dynamic_inventory.py

**Inspec**

# Compliance Testing with InSpec:

• Verify the VM is configured correctly using an InSpec profile:

o Check if nginx is installed and running.

o Validate that the default nginx page contains the required message.

o Ensure SSH root login is disabled.

o Verify the SSH port is set to 22.

o Ensure the devops user exists and is in the sudo group.


# Directory structure of Inspec code :-

├── inspec/

       ├── devops_challenge.rb



 
### Steps to follow for this Github repository

1. Download repository using URL https://github.com/abidulwahab/coding_chalenge.git
2. create your own repository and upload all the files to github main branch, using git commands.
3. Create 3 repository secrets with below names and update values respectively
    AWS_ACCESS_KEY_ID 
    AWS_SECRET_ACCESS_KEY
    AWS_PRIVATE_KEY
   
5. Execute Github actions or commit anything to main branch and pipeline will be executed.
6. Monitor pipeline for any errors.
