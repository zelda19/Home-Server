# Home-Server
A documentation of my home server project using an old HP ProBook 455 G4 laptop with a broken screen, home server running Fedora Server.

![image alr](https://github.com/zelda19/Home-Server/blob/0db94db33163ec7b54e6451ea0dce85ec8ef22f6/jellyfin-dashboard.png)
## Component  Details
Device     HP ProBook 455 G4
CPU        AMD A10-9600P
OS         Fedora Server (minimal, no GUI)
Storage    Internal SSD 256gb / 8gb ram

## Service Installed
Service:   Purpose:
Jellyfin   Media server / streaming
Samba      File sharing over local network

## Setup Steps
 OS Installation
    Downloaded Fedora Server ISO from fedoraproject.org
    copy to ventoy
    Installed Fedora Server
    Selected timezone: (GMT+8)
    Connected to WiFi during installation via the Anaconda

  Jellyfin Media Server
    Installation
    Add RPM Fusion repository
    sudo dnf install jellyfin -y
    sudo systemctl enable --now jellyfin

  Samba File Sharing
    Installation
    sudo dnf install samba -y
    sudo systemctl enable --now smb nmb
    
