---
layout: post
title: "Learning Linux and Networking"
date: 2020-01-28
---



Learning Linux and Networking



A. Setup learning environment

1. Download latest ubuntu LTS version 18.04

2. Install on Virtual Box

3. Increased the VM RAM to 2GB since it did not install properly

4. Run the Virtual BOX GA ios image once logged into the VM after install
(*This enables the fullscreen mode to expand the entire length and breadth of the screen*)

5. Enable sharing folders between host machine and guest

Power off VM
Add a folder to share in the VM settings shared folder
Power on VM

Detailed Explanation from Stackoverflow - https://unix.stackexchange.com/a/156469/391500

Before starting your Guest
Go to VirtualBox Manager
Select your interested Guest
Go to Guest Settings
In Guest Settings, scroll the left side-menu, and go to Shared Folders
In Shared Folders, add your interested folder in the Host machine
After adding your Host folder path, you will see an updated Folders List in Shared Folders. Remember your newly folder Name shown in this list. Say it is HOST_SHARE.
Click OK and save your changes.
Start your Guest machine
In Guest machine, create a new folder, e.g. GUEST_SHARE
In Guest terminal, type

sudo mount -t vboxsf HOST_SHARE GUEST_SHARE`
If you see the error mount: wrong fs type, bad option, bad superblock on …, this means you first need to install virtualbox-guest-utils.

sudo apt-get install virtualbox-guest-utils
Then run the mount command again

You shall find your stuffs in this GUEST_SHARE folder




B. TBC...
