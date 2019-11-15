# File Associations

https://blogs.technet.microsoft.com/windowsinternals/2017/10/25/windows-10-how-to-configure-file-associations-for-it-pros/

For a newer version of Win 10, will need to export an updated association file since it
will likely have additional defaults.

## Windows 10 1809

## Import the file associations manually

From admin command prompt
```
Dism.exe /online /export-defaultappassociations:C:\git\windows-survival\resources\custom_1809.xml
```

## Import file assocations with a task scheduler script

Run with the highes privileges

Program/sript
```
cmd
```

Add arguments
```
/c C:\git\windows-survival\scripts\import_1809_associations.bat
```


## Export file assocations to build a base file

From admin command prompt
```
Dism.exe /online /import-defaultappassociations:C:\git\windows-survival\resources\custom_1809.xml
```
