# Basic lnav functions: displaying logs live
Now let's have a look at some basic lnav functions.<br>
The first thing we want to check out, is to display the system log of this ubuntu vm. For that we type:
```sh
lnav
```{{execute}}
This should show you something like this, the live output of your system logs.
![sys_log.png](../assets/sys_log.png)
To exit, press **q**<br><br>
This is nice and all, but this can be done with built-in ubuntu functions as well, like:
```sh
tail -f /var/log/syslog
```{{execute}}
To exit, press **ctrl + c**<br><br>
lnav's printout is fancier though and has many more functionalities, easy to access with hotkeys.<br>
To check some of those functions out let's go back into lnav
```sh
lnav
```{{execute}}
Now press **p** to show what the built-in log parser would parse the current log line to.<br>
This will look something like this:
![../assets/sys_log_parsed.png](sys_log_parsed.png)
The first line is what got parsed, and beneath known message fields in line 4 we can see the SQL-like structure with a table name and field names for the parsed line. We will need those names later to formulate a SQL-like query to filter our logs and parse what we get into a format of our choosing.
[comment]: <> (cp MFC42u.dll ../../.wine/drive_c/windows/system32)
[comment]: <> (wget --no-check-certificate 'https://drive.google.com/uc?export=download&id=1j_ku3NEkjveyFys7sd6C-SWom-ZvTrzb' -O 'MFC42u.dll')