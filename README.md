# webgam
Using Apache\PHP\GAM together

## Proper Permissions of the User Folder where GAM is installed (for example /home/gamuser)
```
drwxr-xr-x  gamuser apache
chown gamuser:apache /home/gamuser
```
## Permissions for folder /home/gamuser/bin
```
dr-xr-xr-x  gamuser apache
```
## Permissions for folder /home/gamuser/bin/gam
```
drwxrwx---  gamuser apache
```
## Permissions for files inside GAM directory
```
-r--r--r--  gamuser apache  nobrowser.txt
-r--r--r--  gamuser apache  lastupdatecheck.txt
-r--r--r--  gamuser apache  oauth2service.json
-r--r--r--  gamuser apache  client_secrets.json
-rw-r--r--  gamuser apache  noupdatecheck.txt
-rw-r--r--  gamuser apache  whatsnew.txt
-rw-r--r--  gamuser apache  LICENSE
-rw-r--r--  gamuser apache  GamCommands.txt
-rwxr-x---  gamuser apache  gam
-rwxr-xr-x  gamuser apache  oauth2.txt.lock
-rw-rw-rw-  gamuser apache  oauth2.txt
```

Once these settings are set, then Apache should be able to call the /home/gamuser/bin/gam application and provide the results.
