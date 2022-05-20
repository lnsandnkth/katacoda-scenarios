# Setup
Now we install microsoft log parser 2.2
## Install microsoft log parser
Create a directory to download the installer to
```sh
mkdir installer
```{{execute}}
Switch to the newly created directory
```sh
cd installer
```{{execute}}
Download the installer from Microsoft
```sh
wget http://www.microsoft.com/download/en/confirmation.aspx?id=24659
```{{execute}}
Install log parser
```sh
wine start LogParser.msi
```{{execute}}