# Basic lnav functions
Now let's have a look at some basic lnav functions.<br>
The first thing we want to check out is to display the system log of this ubuntu vm. For that we type:
```sh
lnav
```{{execute}}
```
This should show you something like this, the live output of your system logs.
![sys_log.png](../images/sys_log.png)
To exit, type :q and press enter.<br>
This is nice and all, but this can be done with built-in ubuntu functions as well, like:
```sh
tail -f /var/log/syslog
```{{execute}}
To exit, press ctrl + c<br>


[comment]: <> (cp MFC42u.dll ../../.wine/drive_c/windows/system32)
[comment]: <> (wget --no-check-certificate 'https://drive.google.com/uc?export=download&id=1j_ku3NEkjveyFys7sd6C-SWom-ZvTrzb' -O 'MFC42u.dll')