# cmd.exe

To add fonts available to the command prompt, install a True Type font like

-   https://github.com/todylu/monaco.ttf/blob/master/monaco.ttf (right click -> Install (All Users))
-   https://sourceforge.net/projects/dejavu/

In the registry path `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Console\TrueTypeFont`
create a new string with a name `000` and value `Monaco`.

The value must match the font name at `HKLM\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Fonts`.

For each additional font, add a `0`, e.g. `0000` and `00000`.

Restart the command prompt after editing the registry.

https://superuser.com/questions/390933/how-to-add-a-font-to-the-cmd-window-choices-in-windows-7-64-bit

`DejaVu Sans Mono` looks pretty good. Remember to install for all users.

Get others from: https://www.slant.co/topics/7014/~fonts-to-use-in-a-terminal-emulator

Others tested

-   InputMono
-   Inconsolata
-   Iosevka Term
-   Source Code Pro

## robocopy

```
robocopy "D:\source\windows-survival" "D:\destination\windows-survival" /S /Z /R:2 /W:1 /REG
```

-   `/S` - copy sub folders, but not empty ones
-   `/Z` - copy in restartable mode
-   `/R:2` - retry up to two times
-   `/W:1` - wait one seconds between retries
-   `/REG` - save retry options in registry
-   `/MIR` - use instead of /S to mirror (will delete extra files at the destination)

## driverquery
