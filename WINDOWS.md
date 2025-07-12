# Windows
## Commands
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

## Icons
- `%systemroot%\system32\shell32.dll` - default
- `%systemroot%\system32\imageres.dll`
- `%systemroot%\system32\ddores.dll` - devices
- `%systemroot%\system32\pifmgr.dll` - retro
