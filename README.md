# Ansible Playbook Scripts Repository  

This repository contains several **scenario-based Ansible playbook scripts**. Each playbook addresses specific automation tasks, making it easier to manage configurations and deployments across different nodes. Below is a list of scenarios with their corresponding playbook files.

---

## **Table of Contents**

1. [Docker Setup Playbook](#1-docker-setup-playbook)  
2. [Jenkins Installation Playbook](#2-jenkins-installation-playbook)  
3. [User Creation Playbook](#3-user-creation-playbook)  
4. [Git Installation and Repository Cloning](#4-git-installation-and-repository-cloning)  
5. [Maven Installation Playbook](#5-maven-installation-playbook)  

---

## 1. **Docker Setup Playbook**  
This playbook performs the following actions on a target node:  
- **Check if Docker is installed**.  
- **Install Docker** if not present.  
- **Ensure Docker service is enabled and running**.  
- **Pull the `httpd` Docker image**.  
- **Run an `httpd` container** with the name **"webapp"**.

**Playbook Script**:  
[docker_httpd_setup.yml](https://github.com/vithran21/Ansible_Playbook_Script/blob/master/docker_httpd_setup.yml)

---

## 2. **Jenkins Installation Playbook**  
This playbook automates the installation of Jenkins using a shell script:  
- **Create a shell script on the Ansible master node** with commands to install Jenkins.  
- **Copy the shell script** to the worker node.  
- **Run the shell script** on the worker node to complete the Jenkins installation.

**Playbook Script**:  
[install_jenkins_playbook.yml](https://github.com/vithran21/Ansible_Playbook_Script/blob/master/install_jenkins_playbook.yml)

---

## 3. **User Creation Playbook**  
This playbook allows the creation of **multiple users** on a worker node.

**Playbook Script**:  
[creating_multi_users_playbook.yml](https://github.com/vithran21/Ansible_Playbook_Script/blob/master/creating_multi_users_playbook.yml)

---

## 4. **Git Installation and Repository Cloning**  
This playbook covers:  
- **Installing Git** on a worker node.  
- **Cloning a remote repository** on the worker node.

**Playbook Script**:  
[git_install_clone_repo.yml](https://github.com/vithran21/Ansible_Playbook_Script/blob/master/git_install_clone_repo.yml)

---

## 5. **Maven Installation Playbook**  
This playbook installs **Maven** on the worker node.

**Playbook Script**:  
[maven_install_playbook.yml](https://github.com/vithran21/Ansible_Playbook_Script/blob/master/maven_install_playbook.yml)

---

## **How to Use**  
1. Clone the repository and copy the script file needed
2. Run "ansible-playbook file.yml" in ansible master where all ansible configs are available with ssh accessability to worker
   
---

## **Contact**  
Feel free to reach out with any questions or suggestions:  
- **GitHub**: [vithran21](https://github.com/vithran21)  
- **LinkedIn**: [linkedin.com/in/pavithranv-210195vp](https://linkedin.com/in/pavithranv-210195vp)

