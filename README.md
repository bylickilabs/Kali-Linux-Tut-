![kali-wallpaper-2015-v1 1 0](https://user-images.githubusercontent.com/109308073/202898304-52cc44f5-4aba-428e-9d90-55664b10bd0c.jpg)
 
|Kali Linux Tutorial| ![Kali](https://img.shields.io/badge/Kali-268BEE?style=for-the-badge&logo=kalilinux&logoColor=white)|![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)|
|---|---|---|
     
### Overview
|Win-KeX provides a Kali Desktop Experience for Windows Subsystem for Linux (WSL 2) with the following features:|
|---|
- Windowed mode: Launch a Kali Linux desktop in a dedicated window
- Seamless mode: share Windows desktop between Windows and Kali apps and menus
sound support
- Support for unprivileged and root sessions
- Shared clipboard for cut and paste between Kali Linux and Windows apps
- Multi-session support: root window & non-priv window & seamless sessions at the same time
- Fully compatible with WSLg
---
|Installation|
|---|
### Requirements:
- Running Windows 10 version 2004 or later
- Using Windows Terminal

|Install Kali Linux in WSL2|
|---|
### Open PowerShell as Administrator and run:
- Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux

|Reboot|
|---|
### Open PowerShell as Administrator and run:
- dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
- dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart


|Reboot|
|---|
### Download and install the WSL2 Linux kernel from here: [LINK](https://aka.ms/wsl2kernel)

- Open PowerShell as Administrator and run: 

|wsl --set-default-version 2|
|---|
- Installing Kali Linux from the Microsoft Store [LINK](https://apps.microsoft.com/store/detail/kali-linux/9PKR34TNCV07?hl=de-de&gl=de)

---

### To update an existing WSL1 kali-linux installation, type:
- Download SubSystem [LINK](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi)
- Open PowerShell as Administrator and run: 
|wsl --set-version kali-linux 2|
|---|
- Run Kali and complete the initial setup

|Install win-kex via:|
|---|
- sudo apt update
- sudo apt install -y kali-win-kex

|Optional Steps:|
|---|
- If you have enough disk space, you can also upgrade the full package.

|Start the upgrade with the following command!|
|---|
- sudo apt install -y kali-linux-large
