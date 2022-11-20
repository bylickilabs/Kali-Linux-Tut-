|Kali-Linux-Tutorial|
|---|

### Überblick
|Win-KeX bietet eine Kali Desktop Experience für Windows-Subsystem für Linux (WSL 2) mit den folgenden Funktionen:|
|---|
- Fenstermodus: Starten Sie einen Kali Linux-Desktop in einem dedizierten Fenster
- Nahtloser Modus: Teilen Sie den Windows-Desktop zwischen Windows- und Kali-Apps und -Menüs
Sound-Unterstützung
- Unterstützung für nicht privilegierte und Root-Sitzungen
- Gemeinsame Zwischenablage für Ausschneiden und Einfügen zwischen Kali Linux- und Windows-Apps
- Multi-Session-Unterstützung: Root-Fenster & Non-Priv-Fenster & nahtlose Sitzungen gleichzeitig
- Voll kompatibel mit WSLg
---
|Installation|
|---|
### Voraussetzungen:
- Ausführen von Windows 10 Version 2004 oder höher
- Verwendung von Windows Terminal

|Kali Linux in WSL2 installieren|
|---|
### Öffnen Sie PowerShell als Administrator, und führen Sie Folgendes aus:
- Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux

|Neustarten|
|---|
### Öffnen Sie PowerShell als Administrator, und führen Sie Folgendes aus:
- dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
- dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart


|Neustarten|
|---|
### Laden Sie den WSL2 Linux Kernel von hier herunter und installieren Sie ihn: [LINK](https://aka.ms/wsl2kernel)
- Öffnen Sie PowerShell als Administrator und führen Sie Folgendes aus: wsl --set-default-version 2
- Installieren von Kali Linux aus dem Microsoft Store https://apps.microsoft.com/store/detail/kali-linux/9PKR34TNCV07?hl=de-de&gl=de

### Um eine vorhandene WSL1 kali-linux-Installation zu aktualisieren, geben Sie Folgendes ein: 
|wsl --set-version kali-linux 2|
|---|
- Führen Sie Kali aus und schließen Sie die Ersteinrichtung ab

|Installieren Sie win-kex über:|
|---|
- sudo apt update
- sudo apt install -y kali-win-kex

|Optionale Schritte:|
|---|
- Wenn sie über genug Speicherplatz verfügen, können sie auch das volle Paket Upgrade durch führen. 

|Mit dem folgendem Befehl starten sie das Upgrade!|
|---|
- sudo apt install -y kali-linux-large

