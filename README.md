# KALIMA ANSIBLE - Bootstraping a fresh Kali VM.

## Ansible offspring of https://github.com/kussic/kalima 

**First ever attempt in ansible so the layout might be completely wrong**

The playbook consists of 4 roles:

1. Bootstrap
	- Update system
	- Remove useless Kali diretories
	- Create project folders layout
	- Mount shared folders
2. Install base tools
	- Too many to list - See the list at /roles/install_base_tools/tasks/. Installation of tools that i find useful. 
3. Remove base tools
	- Too many to list - See the list at /roles/remove_base_tools/tasks/. Kept this here for future reference if i want to exclude some tools
4. Various utilities installation
	- Install fish and omf
	- Setup bash greeting
	- Setup wallpaper
	- Disable beeps and screensaver
5. Kali Silencer
	- Disable automatic updated
	- Stop NTP service
	- Disable RPCBind
	- Stop network services
	- Disable ICMP echo replies
	- Disable IPv6
	- Silence Firefox