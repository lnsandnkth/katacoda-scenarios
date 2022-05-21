# Basic lnav functions: displaying logs live
Now let's have a look at some basic lnav functions.<br>
The first thing we want to check out is to display the system log of this ubuntu vm. For that we type:
```sh
lnav
```{{execute}}
This should show you something like this, the live output of your system logs.
![sys_log.png](../images/sys_log.png)
To exit, press **q**<br>
This is nice and all, but this can be done with built-in ubuntu functions as well, like:
```sh
tail -f /var/log/syslog
```{{execute}}
To exit, press **ctrl + c**<br>
lnav's printout is fancier though and has many more functionalities, easy to access with hotkeys.<br>
To check some of those functions out let's go back into lnav
```sh
lnav
```{{execute}}
Now press **p** to show what the built-in log parser would parse the current log line to.
[comment]: <> (cp MFC42u.dll ../../.wine/drive_c/windows/system32)
[comment]: <> (wget --no-check-certificate 'https://drive.google.com/uc?export=download&id=1j_ku3NEkjveyFys7sd6C-SWom-ZvTrzb' -O 'MFC42u.dll')