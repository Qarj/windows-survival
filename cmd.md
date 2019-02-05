# cmd.exe

## robocopy

```
robocopy D:\source D:\destination /S /Z /R:2 /W:1 /REG
```
- `/S` - copy sub folders, but not empty ones
- `/Z` - copy in restartable mode
- `/R:2` - retry up to two times
- `/W:1` - wait one seconds between retries
- `/REG` - save retry options in registry
- `/MIR` - use instead of /S to mirror (will delete extra files at the destination)
