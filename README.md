# InstallUbuntuDualBoot

- disable secure boot
- Swith SATA mode to ARCH from Raid on ( firt go to safe mode in windows, then restart, go to bios, change to ARC, come to windows,change form safe mode to normal, restart)
- I think no nee to desable TMP
- If not using UBS, create a bootable mount on another volume, not on the same where Ubuntu will be installed
- use Universal-USB-Installer-2.0.0.1 to write ISO file in the created bootable mount
- if boot option is not showing, add grubx64.ext file from efi/boot folder. to do this in bios, go to boot secton, add boot from file (or something like this)
- Instaed of installing go to try ubutu and install once inside ubuntu


_ To mount linux drive automatically on wsl create a scheduler with highest privlidge and folowing command  . browse C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe in program and put follwing in arg
 `-ExecutionPolicy Bypass -command  "wsl --mount \\.\PHYSICALDRIVE1  --partition 2"` 
