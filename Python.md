# Python 3 environment variables

## Environment variables
Set environment variable `PYTHONPATH`
```
C:\Python36-32\Scripts\;C:\Python36-32\;C:\Python36-32\Lib;C:\Python36-32\DLLs
```
Add to end of system path.


## File association

ver.py
```
import sys
print(sys.version)
print(sys.executable)
```

Default for key `HKEY_CLASSES_ROOT\.py` probably has data `Python.File`
so set `HKEY_CLASSES_ROOT\Python.File\Shell\open\command` to `"C:\python36-32\python.exe" "%1" %*`

https://superuser.com/questions/433897/python-in-command-line-runs-the-wrong-version


## Virtual environments

Create
```
python -m venv %systemdrive%%homepath%\my-venv
```

Activate
```
%systemdrive%%homepath%\my-venv\Scripts\activate.bat
```

Deactivate
```
deactivate
```

https://www.techcoil.com/blog/how-to-create-a-python-3-virtual-environment-in-windows-10/

