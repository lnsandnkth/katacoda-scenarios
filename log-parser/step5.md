## Creating a shell script to store the parsed logs automatically and call it via a cron job every day
First create the shell script that stores the output in a file called table.csv, instead of just printing the results to the standard output.
```sh
printf "lnav -n \
    -c ';SELECT log_procname, count(*) AS total FROM syslog_log GROUP BY log_procname ORDER BY total DESC LIMIT 10' \
    -c ':write-csv-to table.csv' \
    /var/log/syslog" > syslogs_top_10_programs.sh
```{{execute}}
Now let's give the script permsisions so we can run it
```sh
chmod 777 ./syslogs_top_10_programs.sh
```{{execute}}
Now run the script to see if it works.
```sh
./syslogs_top_10_programs.sh
```{{execute}}
It should have printed the results to the standard out and also created the table.csv file. Check it out in the window above the console, after the view has refreshed.
<br>
Now you can reuse that script however you like. But we are gonna create a so called cron job that lets the virtual machine execute that script once every day at 3am.<br>
For that we edit the list of cron jobs via:
```sh
crontab -e
```{{execute}}
Now append this line:
```sh
0 3 * * * /usr/bin/sh /root/syslogs_top_10_programs.sh
```{{copy}}
Press **ctrl + x**, then press **y** and then **enter**, to save the changes.<br>
The first 5 variables "0 3 * * *" stand for the time the job should be executed in the format: Minute (0-59), Hour(0-23), Day of Month(1-31), Month(1-12), and Day of Week(Sunday=0-7).<br> 
(Note: I couldn't get this cron job running on katacoda, simpler ones worked but not this one, on your local ubuntu install it should work though)