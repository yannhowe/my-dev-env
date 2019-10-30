# My Dev Environment
This documents how I run my development environment. I'm primarily a systems guy who dabbles in the application world so that shapes how I build and run solutions to get things done in a major way. 

There are enough off the shelf capabilities packaged as docker images which allow me to write minimal code to integrate these capabilities to customize and create something useful.

## Main Pieces
- Docker
- Docker Compose
- Python 3
- Pipenv
- Django

## Setting up on Windows 10
### Get windows subsystem for linux

1. In PowerShell:
```
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```
2. Reboot
3. Go to the microsoft store and install [Ubuntu 16.04](https://www.microsoft.com/store/apps/9pjn388hp8c9)
4. Install a whole bunch of software from Powershell:
```
# Install Chocolatey
Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))

# Install software
choco install git 7zip mremoteng telegram whatsapp vmware-powercli-psmodule bosh-cli vmwarevsphereclient govc kubernetes-cli docker-compose docker-desktop  kubernetes-helm vscode vscode-gitlens vscode-docker vscode-gitignore terraform
```
5. Go [here](https://nickjanetakis.com/blog/setting-up-docker-for-windows-and-wsl-to-work-flawlessly) and get WSL to work with docker desktop "flawlessly"
