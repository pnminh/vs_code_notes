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

Go to `View > Command Pallete (or Ctr+Shift+P)` and search for the command `Remote-SSH: Connect to host...`   
![Connect Remote-SSH](media/4_connect_remote_ssh.png)

