# Fedora 31 post-installation

Ansible playbook that runs post-fedora-31 workstation setup:

* Installs ansible so we can run the rest of the script (and re-run) (in run.sh)
* Enables dnf fast-mirror and increases parallel downloads.
* Makes your sudo password-less
* Installes: htop, glances, vim-enahcned, powerline, unzip, java, java web plugin for firefox, tmux
* Enables some nice short cuts with git
* Increases Bash history and adds timestamp
* Reduces kernel swapiness (better performance)
* Applies some nice vim defaults (/etc/vimrc.more).
* Adds rpmfusion, adobe(flash), skype4linux and google chrome repos
* Installs flash, skype4linux, vlc and google-chrome
* Removes chines/tamel and other south-east-asian fonts
* Enables playing mp3 and other multimedia codecs.
* Configures gnome top par to show seconds and date
* Disables default menu in gnome Terminal
* Disables gnome tracker [optional defaults to no]
* Installs additional development packages [optional defaults to yes]

To run:

Clone this repository or download the zip file and unzip, then cd into the new folder.

Then as a sudo-enabled user run:

(it may ask for the sudo password twice)

`./run.sh`

Then run 
`./user.sh`

Then reboot your computer

Note: To enable/disable optional steps edit the flags in vars.yml
