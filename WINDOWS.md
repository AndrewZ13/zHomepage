# Windows
## Commands
### Software
- `msix`/`msixbundle`: `Add-AppPackage -Path "..."`

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
