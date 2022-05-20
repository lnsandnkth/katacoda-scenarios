# Setup
First we need to install wine, in order to run microsoft log parser on ubuntu to parse our logs.
## Install wine
install the latest stable wine distribution
```sh
sudo apt-get install wine64
```{{copy}}
install a wine helper script for extra runtime libraries needed to run log parser<br>
(Log parser needs the MFC42u.dll; you could also install that manually)
```sh
sudo apt-get install winetricks
```{{copy}}
```sh
mkdir gecko
cd gecko
wget http://dl.winehq.org/wine/wine-gecko/2.47.2/wine-gecko-2.47.2-x86_64.msi
wine start wine-gecko-2.47.2-x86_64.msi
```
