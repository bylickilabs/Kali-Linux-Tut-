![kali-wallpaper-2015-v1 1 0](https://user-images.githubusercontent.com/109308073/202898304-52cc44f5-4aba-428e-9d90-55664b10bd0c.jpg)
 
|Kali Linux Tutorial| ![Kali](https://img.shields.io/badge/Kali-268BEE?style=for-the-badge&logo=kalilinux&logoColor=white)|
|---|---|
     
### Überblick
|Win-KeX bietet ein Kali-Desktop-Erlebnis für das Windows-Subsystem für Linux (WSL 2) mit den folgenden Funktionen:|
|---|
- Fenstermodus: Starten Sie einen Kali Linux-Desktop in einem speziellen Fenster
- Nahtloser Modus: Teilen Sie den Windows-Desktop zwischen Windows- und Kali-Apps und -Menüs
solide Unterstützung
- Unterstützung für unprivilegierte und Root-Sitzungen
- Gemeinsame Zwischenablage zum Ausschneiden und Einfügen zwischen Kali Linux- und Windows-Apps
- Multi-Session-Unterstützung: Root-Fenster und nicht-privates Fenster sowie nahtlose Sitzungen gleichzeitig
- Vollständig kompatibel mit WSLg
---
|Installation|
|---|
### Anforderungen:
- Ausführen von Windows 10 Version 2004 oder höher
- Verwendung des Windows-Terminals

|Installieren Sie Kali Linux in WSL2|
|---|
### Öffnen Sie PowerShell als Administrator und führen Sie Folgendes aus:
- Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux

|Neustart|
|---|
### Öffnen Sie PowerShell als Administrator und führen Sie Folgendes aus:
- dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
- dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart


|Neustart|
|---|
### Laden Sie den WSL2-Linux-Kernel hier herunter und installieren Sie ihn: [LINK](https://aka.ms/wsl2kernel)

- Öffnen Sie PowerShell als Administrator und führen Sie Folgendes aus:

|wsl --set-default-version 2|
|---|
- Installation von Kali Linux aus dem Microsoft Store [LINK](https://apps.microsoft.com/store/detail/kali-linux/9PKR34TNCV07?hl=de-de&gl=de)

---

### Um eine vorhandene WSL1-Kali-Linux-Installation zu aktualisieren, geben Sie Folgendes ein:
- SubSystem herunterladen [LINK](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi)
- Öffnen Sie PowerShell als Administrator und führen Sie Folgendes aus:

|wsl --set-version kali-linux 2|
|---|
- Führen Sie Kali aus und schließen Sie die Ersteinrichtung ab

|Win-kex installieren über:|
|---|
- Sudo apt-Update
- sudo apt install -y kali-win-kex

|Optionale Schritte:|
|---|
- Wenn Sie über genügend Speicherplatz verfügen, können Sie auch das Gesamtpaket upgraden.

|Starten Sie das Upgrade mit dem folgenden Befehl!|
|---|
- sudo apt install -y kali-linux-large
