# Setup
First we need to install wine, in order to run microsoft log parser on ubuntu to parse our logs.
## Install wine
install the latest stable wine distribution
```sh
sudo apt-get install wine64
```{{copy}}
install a wine helper script for extra runtime libraries needed to run log parser<br>
```sh
sudo apt-get install winetricks
```{{copy}}