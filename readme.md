# Ansible Dynamic Inventory for AWS EC2

This repository contains the necessary configurations and playbooks to manage AWS EC2 instances using Ansible's dynamic inventory feature.

### Prerequisites

- **Ansible**: Make sure you have Ansible installed on your system.
- **AWS CLI**: Ensure AWS CLI is configured with the necessary credentials and access to your AWS environment.

### Setup Instructions

#### Step 1: Configure Dynamic Inventory in `ansible.cfg`

To begin using Ansible with AWS EC2 instances, you need to configure the dynamic inventory in your `ansible.cfg` file.

1. **Add the following configuration**:

```ini
[defaults]
inventory = ./aws_ec2.yml

``` 
**Running the playbook** :

```
ansible-playbook -i aws_ec2.yml main.yml

```