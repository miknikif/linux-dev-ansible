<img src="https://raw.githubusercontent.com/geerlingguy/mac-dev-playbook/master/files/Mac-Dev-Playbook-Logo.png" width="250" height="156" alt="Mac Dev Playbook Logo" />

# Linux Development Ansible Playbook

This playbook installs and configures most of the software I use on my Linux for web and software development. Some things in linux are slightly difficult to automate, so I still have a few manual installation steps, but at least it's all documented here.

## Installation

  1. [Install Ansible](https://docs.ansible.com/ansible/latest/installation_guide/index.html):

     1. Run the following command to add Python 3 to your $PATH: `export PATH="$HOME/Library/Python/3.8/bin:/opt/homebrew/bin:$PATH"`
     2. Upgrade Pip: `sudo pip3 install --upgrade pip`
     3. Install Ansible: `pip3 install ansible`

  2. Clone or download this repository to your local drive.
  3. Run `ansible-galaxy install -r requirements.yml` inside this directory to install required Ansible roles.
  4. Run `ansible-playbook main.yml --ask-become-pass` inside this directory. Enter your Linux account password when prompted for the 'BECOME' password.
