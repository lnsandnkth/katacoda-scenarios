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
Download the installer from my google drive
```sh
wget https://drive.google.com/uc?export=download&id=1NrvQF7J1eTnFyvglw6pbMOy-tK56HqWc
```{{copy}}
This is already the installed log parser
```sh
sudo apt-get install unzip
unzip "Log Parser 2.2.zip"
cd "Log Parser 2.2"
wine start LogParser.exe
```{{copy}}