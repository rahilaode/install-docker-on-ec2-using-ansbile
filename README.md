# Install Docker & Docker Compose on a Remote Server using Ansible

This guide demonstrates the process of installing and configuring Docker and Docker Compose on a remote server using Ansible. Ansible is a powerful tool that automates software provisioning, configuration management, and application deployment.

## Overview

Docker is a set of platform as a service products that use OS-level virtualization to deliver software in packages called containers. Docker Compose is a tool for defining and running multi-container Docker applications. With Compose, you use a YAML file to configure your application's services, networks, and volumes.

The purpose of this project is to simplify the setup of Docker and Docker Compose on any remote server using Ansible, making it easy to replicate environments and ensure consistency across multiple setups.

## Prerequisites

- A remote server with SSH access.
- Ansible installed on your local machine.

## Quick Start

1. **Clone the Repository:**
   Clone this repository to your local machine to get started with the setup.
   ```
   git clone git@github.com:rahilaode/install-docker-on-ec2-using-ansbile.git
   ```

2. **Set Up Inventory:**
   Modify the `inventory` file to include the IP address of your remote server.

3. **Run Ansible Playbook:**
   Execute the Ansible playbook to install Docker and Docker Compose on your remote server.
   ```
   ansible-playbook -i inventory playbooks/install-docker-playbook.yml 
   ```


## What is Ansible?

Ansible is an open-source tool that provides a suite of software tools for automating software provisioning, configuration management, and application deployment. Ansible uses a simple syntax written in YAML called playbooks. Ansible communicates over normal SSH channels to retrieve information from remote machines, manage files, and execute commands.

## Conclusion

By following this guide, you can automate the installation and configuration of Docker and Docker Compose on any remote server using Ansible. This approach not only saves time but also ensures that the environments are consistent and reproducible.

For more detailed instructions and configurations, refer to the official Ansible documentation at [Ansible Documentation](https://docs.ansible.com/).