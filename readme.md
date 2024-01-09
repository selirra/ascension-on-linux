# :)

## Installing Dependencies 

### Arch 
```
sudo pacman -Syu 
sudo pacman -S wine winetricks mono 
```

### Debian/Ubuntu 
```
sudo apt update -qq 
sudo apt install -qqy wine winetricks mono-complete 
```

### CentOS
```
sudo yum update -q 
sudo yum install -qy wine winetricks mono-complete 
```

## Setting up Ascension WINE bottle 
```
export WINEPREFIX="/home/$USER/.config/projectascension/WoW"
export WINEARCH=win32
```

## Installing dependencies for WINE
```
mkdir -p /home/$USER/.config/projectascension/WoW && cd /home/$USER/.config/projectascension
wget https://dl.winehq.org/wine/wine-mono/6.3.0/wine-mono-6.3.0-x86.msi
wine msiexec /i wine-mono-6.3.0-x86.msi
winetricks win10 ie8 corefonts dotnet45 vcrun2015
```
