# Workstation

Software setup for my development desktop.

It was tested on latest Ubuntu LTS release in 2015, but now is no longer supported.

## Setup

0. Install latest stable ansible

    ```bash
    sudo apt-add-repository ppa:ansible/ansible
    sudo apt-get update
    sudo apt-get install ansible
    ```
    
1. Clone this repository

    ```bash
    git clone https://github.com/aeryaguzov/workstation.git /path/to/working/dir && cd /path/to/working/dir
    ```

2. Setup hosts

    ``` bash
    cp hosts.example hosts
    ```
    You need to be a template engine for a while and replace vars (**{{var}}**) with credentials for your workstation
    
3. Run playbook and stay strong until ansible gets all done!

    ```bash
    ansible-playbook workstation.yml
    ```

