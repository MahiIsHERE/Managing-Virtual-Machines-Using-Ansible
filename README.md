# Managing-Virtual-Machines-Using-Ansible
Managing Virtual Machines of Virtual Box Using Ansible

Explanation:
In the VirtualBox directory C:\Program Files\Oracle\VirtualBox:
VBoxManage.exe is a command-line utility that allows to control all aspects of VirtualBox like managing VMs (start, stop, configure), controling VirtualBox settings, and automating tasks through scripts. 
Here, it is used to manage the lifecycle of a VirtualBox VM running on the Windows machine & query the status of a VM (showvminfo), start a VM (startvm), and power off a VM (controlvm). 

The commands used are:
VBoxManage showvminfo <VM_name>: Displays detailed information about a specified VM, including its running status.
VBoxManage startvm <VM_name> --type headless: Starts the specified VM in headless mode (without a GUI).
VBoxManage controlvm <VM_name> poweroff: Powers off the specified VM.

Requirements:
Before starting, we have to install ansible by:
pip install ansible
and ensure it is installed correctly using:
ansible --version
then:
wsl --list --verbose
  NAME              STATE           VERSION
* Ubuntu            Running         2
wsl -d Ubuntu
root@DESKTOP-FPNNIGS
