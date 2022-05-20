# Setup
Now we install microsoft log parser 2.2
## Install microsoft log parser
Create a directory to download the installer to
```sh
mkdir installer
```{{copy}}
Switch to the newly created directory
```sh
cd installer
```{{copy}}
Download the installer from Microsoft
```sh
wget https://download.microsoft.com/download/f/f/1/ff1819f9-f702-48a5-bbc7-c9656bc74de8/LogParser.msi
```{{copy}}
Install log parser
```sh
wine start LogParser.msi
```{{copy}}