# Setup
First we need to install wine, in order to run microsoft log parser on ubuntu to parse our logs.
## Install wine
install the latest stable wine distribution
```sh
sudo apt-get install wine7.0
```{{execute}}
install a wine helper script for extra runtime libraries needed to run log parser<br>
(Log parser needs the MFC42u.dll; you could also install that manually)
```sh
sudo apt-get install winetricks
```{{execute}}
