# SSH Workspace
## Install VsCode
On Fedora/RHEL/CentOS
```bash
$ sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
$ sudo sh -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/vscode.repo'
$ sudo dnf check-update
$ sudo dnf install code
$ code
```
Go to extension menu (`Ctrl+Shift+X`)   
![Extension menu](media/1_extension_menu.png)

Search for and select `Remote-SSH` extension from Microsoft (should be the first one from the list)   
![Search Remote-SSH](media/2_search_remote_ssh.png)

Install the extension   
![Install Remote-SSH](media/3_install_remote_ssh.png)

Go to `View > Command Pallete (or Ctr+Shift+P)` and search for the command `Remote-SSH: Connect to host...`  to run a SSH session or `Remote-SSH: Add New SSH Host` to persist the host configurations for future usage.  
![Connect Remote-SSH](media/4_connect_remote_ssh.png)

Input the hostname and enter. Add password/ssh key location when prompted      
![Add Remote-SSH](media/5_add_host_remote_ssh.png)

After vscode connects successfully to the hostname, we should see the hostname at the bottom left. Also go to `Terminal > New Terminal` will give us the direct ssh session with the host.    
![Terminal in Remote-SSH](media/6_terminal_remote_ssh.png)

We then can have our remote workspace run on the host machine. Select `File > Open Folder (Ctrl+O)` to open the workspace   
![Open folder in Remote-SSH](media/7_open_folder_remote_ssh.png)

We can also install extensions on the remote workspace such as `yaml` from Red Hat and `kubernetes`   
![Other extensions in Remote-SSH](media/8_other_extensions_remote_ssh.png)

