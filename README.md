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