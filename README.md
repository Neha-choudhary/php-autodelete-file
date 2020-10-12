## PHP Auto Delete File with CronJob
How to use:
- Set up database connection.
- Save the autodelete.php file in the root directory.
- On cPanel open the CronJob menu.
- Set the common settings of cronjob.<br>
<b>Minute : 0</b><br>
<b>Hour : 0</b><br>
<b>Day : *</b><br>
<b>Month : *</b><br>
<b>Weekday : 0</b>
- Then enter the following Command.<br>
```
/usr/local/bin/php /home/yourname/public_html/autodelete.php
```
If you are using a local server you can use the terminal by entering the following command.<br>
```
sudo crontab -e
```
Then enter the following command.<br>
```
0 0 * * 0 /usr/local/bin/php /var/www/html/yourfolder/autodelete.php
```
The command above will run the autodelete.php file every 1 month at 00:00 AM.
