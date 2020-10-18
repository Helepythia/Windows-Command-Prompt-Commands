# Windows-Command-Prompt-Commands
Below add some helpful commands that you regularly use, what they do and what they're typically used for.


#sfc /scannow, System file checker will help repair the Windows OS.
sfc /scannow


#Powershell Command: Below will reinstall your Windows 10 Apps, in case they mess up. Do note that this will help fix your start menu, in case it messes up and does not seem to function. 

Get-AppXPackage | Foreach {Add-AppxPackage -DisableDevelopmentMode -Register "$($_.InstallLocation)\AppXManifest.xml"
