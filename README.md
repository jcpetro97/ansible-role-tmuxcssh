# TmuxCsshInstall

This is an ansible role that installs tmux-cssh from github

#### Variables

Variables can be set in a few ways.  
*  **vars/main.yml** from the main playbook that calls this role
*  passed in directly when the role is called(see below)
*  **TmuxCsshInstall/vars/main.yml** file.  

The URL for the file needs to be set in one of the vars files.  The variable should be named **TmuxCsshUrl**

#### example of how to call this role

If you pass the variables in directly

```
	roles:
      - {role: TmuxCsshInstall, UserName: "testuser"} 

```

If the variables are stored in a vars file:

```
	roles:
		- TmuxCsshInstall
```