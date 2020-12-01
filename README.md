# macos-config

## Install
The easiest way to install is to follow the following steps:

1. Make sure you have signed into the Mac App Store.  This makes mas easier to deal with
2. Install Apples's command line tools: `xcode-select --install`
3. Upgrade Pip to 20.3 or later: `sudo pip3 install --upgrade pip`
4. Install Ansible: `sudo pip install ansible`
5. Create the mac-ansible directory `mkdir mac-ansible`
6. Change directory to mac-ansible `cd mac-ansible`
7. Clone the Repository: `git clone https://github.com/AustinCloudGuru/macos-config`
8. Change Directories into the repo: `cd mac-playbook`
9. Update the requirements file: `ansible-galaxy install -r requirements.yml`
10. Run the osascript command to account for sandboxing ` osascript -e 'tell application "Finder"' -e 'set _b to bounds of window of desktop' -e 'end tell'`
11. Run the Playbook: `ansible-playbook playbook.yml -i inventory -K`

Commands:

     xcode-select --install
     sudo pip3 install --upgrade pip
     sudo pip install ansible
     mkdir mac-ansible 
     cd mac-ansible 
     git clone https://github.com/AustinCloudGuru/macos-config
     cd macos-config
     ansible-galaxy install -r requirements.yml
     osascript -e 'tell application "Finder"' -e 'set _b to bounds of window of desktop' -e 'end tell'
     ansible-playbook playbook.yml -i inventory -K
