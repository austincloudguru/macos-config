# macos-config

## Install
The easiest way to install is to follow the following steps:

1. Make sure you have signed into the Mac App Store.  This makes mas easier to deal with
2. Install Apples's command line tools: `xcode-select --install`
3. Install Pip: `sudo easy_install pip`
4. Install Ansible: `sudo pip install ansible`
5. Clone the Repository: `git clone https://github.com/AustinCloudGuru/mac-playbook`
6. Change Directories into the repo: `cd mac-playbook`
7. Update the requirements file: `ansible-galaxy install -r requirements.yml`
7. Run the Playbook: `ansible-playbook playbook.yml -i inventory -K`

Commands:

     xcode-select --install
     sudo easy_install pip
     sudo pip install ansible
     git clone https://github.com/AustinCloudGuru/mac-playbook
     cd macos-config
     ansible-galaxy install -r requirements.yml
     ansible-playbook playbook.yml -i inventory -K