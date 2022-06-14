# Workstation Tools

This repository contains scripts to automate and speedup the workflow and preparation for my machine.

> **_Disclaimer_** :  
> Those scripts are ubuntu related with major version 18+, for other distributions you'll need to adapt it
___
## Prepare Workstation

> Read the `ubuntu.yml` file before applying and be sure to understand everything that will be done.

1. Install Ansible
```bash
sudo apt update && sudo apt install ansible unzip git -y
```
2. Clone this repository
```bash
git clone https://gitlab.intelie.com/sre/development.git
```
3. Browse to folder development/aleon.chagas/setup-linux

4. Apply the configuration
```
ansible-playbook setup/ubuntu.yml --ask-become-pass
```
>Type your password when asked to give root permissions for some actions.
___

5. Set Tilix as default when pressing CRLT+ALT+T
```bash
sudo update-alternatives --config x-terminal-emulator
```

6. Adjust Flameshot
> Keyboard Shortcuts > New > Name: flameshot Command: flameshot Gui Shortcut: SHIFT+SUPER+S
___

1. Adjust VIM
```bash
sudo vim /etc/vim/vimrc +$
```
```
" YAML Resourses

set cursorline
set cursorcolumn
set number
set paste
```
