# Ansible-Deploy-AWS-EC2-Instance

Launch aws ec2 instance using Ansible Playbook

## Prerequisite

-[Install AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-install.html)

-[Install Boto3 and Set Amazon EC2 Keys(macOS)](https://crunchify.com/how-to-install-boto3-and-set-amazon-keys-a-python-interface-to-amazon-web-services/)

-[Install Python](https://installpython3.com/mac/)

## Run Project

Command: ansible-playbook site.yml 

## Options

To make playbook more flexible and interactive, you can delete vars section and pass the same variables on playbook execution.

Command: ansible-playbook site.yml -e instance_type=t2.micro -e security_group=WebServers -e image=ami-0080e4c5bc078760e -e region=us-east-1 -e count=1
