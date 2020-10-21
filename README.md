# Windows-Command-Prompt-Commands
Below add some helpful commands that you regularly use, what they do and what they're typically used for.


#sfc /scannow, System file checker will help repair Windows OS.

sfc /scannow

#Dism, Use this to help repair Windows OS.

DISM /Online /Cleanup-Image /ScanHealth


#Powershell Command: Below will reinstall your Windows 10 Apps, in case they mess up. Do note that this will help fix your start menu, in case it messes up and does not seem to function. 

Get-AppXPackage | Foreach {Add-AppxPackage -DisableDevelopmentMode -Register "$($_.InstallLocation)\AppXManifest.xml"


#ipconfig, A small script in case your internet/DNS fails. That's to say, if somehow your pc is not working, and yet your phone is (and they're both on the same wifi) you use this whole set of commands.
ipconfig /flushdns
ipconfig /registerdns
ipconfig /release
ipconfig /renew
