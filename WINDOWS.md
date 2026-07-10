# Windows
## Commands
### PS
1. `Set-ExecutionPolicy RemoteSigned`
2. `Set-ExecutionPolicy Restricted`

### GP
0. Export: `LGPO.exe /b "X:\GP"`
1. Import: `LGPO.exe /g "X:\GP\{...}"`
2. Reload: `gpupdate.exe /force`

### Software
Install `msix`/`msixbundle`/`appx` files:
- `Add-AppxPackage -Path "..."`

#### Dependencies
- [Microsoft.VCLibs.x64.14.00.Desktop.appx](https://aka.ms/Microsoft.VCLibs.x64.14.00.Desktop.appx)
- [Microsoft.VCLibs.x86.14.00.Desktop.appx](https://aka.ms/Microsoft.VCLibs.x86.14.00.Desktop.appx)

### Shutdown
- `shutdown -s -t [Seconds]`
- `shutdown -a` to abort

### Maintenance
- `DISM.exe /Online /Cleanup-image /Restorehealth`
- `sfc /scannow`

### Restore Classic Context Menu
- Do: `reg.exe add "HKCU\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}\InprocServer32" /f /ve`
- Undo: `reg.exe delete "HKCU\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}" /f`

## Icons
- `%systemroot%\system32\shell32.dll` - default
- `%systemroot%\system32\imageres.dll`
- `%systemroot%\system32\ddores.dll` - devices
- `%systemroot%\system32\pifmgr.dll` - retro
