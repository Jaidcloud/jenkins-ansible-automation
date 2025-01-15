# jenkins-ansible-automation
To automate the deployment of Jenkins on AWS EC2 instances using Ansible.

# Automating Jenkins Deployment on AWS EC2 with Ansible

This repository contains an Ansible playbook and role that automates the deployment of Jenkins on AWS EC2 instances. The playbook installs Java, configures Jenkins, and ensures that Jenkins is accessible via the EC2 instance's public IP. The purpose of this automation is to provide a consistent, repeatable, and scalable Jenkins deployment process.

## Prerequisites

Before running the playbook, ensure the following:

1. **AWS Account**: You need an AWS account to provision EC2 instances.
2. **Ansible**: Ansible must be installed on your local machine. You can install it using the command below (for Ubuntu):
    ```bash
    sudo apt update
    sudo apt install ansible
    ```
3. **EC2 Instance**: A running EC2 instance with Ubuntu Server 20.04 LTS (or other compatible Ubuntu versions).
4. **SSH Key Pair**: A valid SSH key pair to access your EC2 instance.
5. **Public IP**: The public IP address of your EC2 instance.
6. **AWS CLI (optional)**: If you want to interact with AWS directly from the command line, you can install AWS CLI:
    ```bash
    sudo apt install awscli
    ```

## Setup

### 1. Clone the Repository

Clone this repository to your local machine:

```bash
git clone https://github.com/yourusername/Jenkins-Automation.git
cd Jenkins-Automation

