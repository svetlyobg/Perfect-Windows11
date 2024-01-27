# Perfect-Windows11
 Perfect Windows 11 is a GitHub repository that provides a comprehensive guide to Windows 11. It includes tips and tricks for various aspects of the operating system

## Bring Back Windows Photo Viewer

Save the folllwing as a `.reg` file

```console
Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\SOFTWARE\Classes\.bmp]
@=”PhotoViewer.FileAssoc.Tiff”

[HKEY_CURRENT_USER\SOFTWARE\Classes\.gif]
@=”PhotoViewer.FileAssoc.Tiff”

[HKEY_CURRENT_USER\SOFTWARE\Classes\.ico]
@=”PhotoViewer.FileAssoc.Tiff”

[HKEY_CURRENT_USER\SOFTWARE\Classes\.jpeg]
@=”PhotoViewer.FileAssoc.Tiff”

[HKEY_CURRENT_USER\SOFTWARE\Classes\.jpg]
@=”PhotoViewer.FileAssoc.Tiff”

[HKEY_CURRENT_USER\SOFTWARE\Classes\.png]
@=”PhotoViewer.FileAssoc.Tiff”

[HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\FileExts\.gif\OpenWithProgids]
“PhotoViewer.FileAssoc.Tiff”=hex(0):

[HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\FileExts\.ico\OpenWithProgids]
“PhotoViewer.FileAssoc.Tiff”=hex(0):

[HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\FileExts\.jpeg\OpenWithProgids]
“PhotoViewer.FileAssoc.Tiff”=hex(0):

[HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\FileExts\.bmp\OpenWithProgids]
“PhotoViewer.FileAssoc.Tiff”=hex(0):

[HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\FileExts\.jpg\OpenWithProgids]
“PhotoViewer.FileAssoc.Tiff”=hex(0):

[HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\FileExts\.png\OpenWithProgids]
“PhotoViewer.FileAssoc.Tiff”=hex(0):
```

Source :: [Britec's Website](https://briteccomputers.co.uk/posts/5-best-registry-hacks-for-windows-11-2/)

## Add a Program to the Context Menu

```cmd
reg add "HKEY_CLASSES_ROOT\Directory\Background\shell\Notepad" /ve /d "Open with Notepad" /f
reg add "HKEY_CLASSES_ROOT\Directory\Background\shell\Notepad\command" /ve /d "C:\Windows\notepad.exe" /f
```

## Disable Bing Search from the Start Menu

```cmd
reg add reg add "HKEY_CURRENT_USER\Software\Policies\Microsoft\Windows\Explorer" /v DisableSearchBoxSuggestions /t REG_DWORD /d 1 /f
```

## Bring the Old Context Menu Back

```cmd
reg add "HKEY_CURRENT_USER\SOFTWARE\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}\InprocServer32" /ve /d "-" /f
```

## Stop Automatic Updates on Windows 11

```cmd
reg add reg add "HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\WindowsUpdate" /f


```

Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\WindowsUpdate