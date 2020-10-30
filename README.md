<h1># Windows-Command-Prompt-Commands</h1>
Below add some helpful commands that you regularly use, what they do and what they're typically used for.


<h2>#sfc /scannow, System file checker will help repair Windows OS.</h2>

sfc /scannow

<h2>#Dism, Use this to help repair Windows OS.</h2>

DISM /Online /Cleanup-Image /ScanHealth


<h2>#Powershell Command: Below will reinstall your Windows 10 Apps, in case they mess up. Do note that this will help fix your start menu, in case it messes up and does not seem to function.</h2>

Get-AppXPackage | Foreach {Add-AppxPackage -DisableDevelopmentMode -Register "$($_.InstallLocation)\AppXManifest.xml"


<h2>#ipconfig, A small script in case your internet/DNS fails. That's to say, if somehow your pc is not working, and yet your phone is (and they're both on the same wifi) you use this whole set of commands.</h2>

ipconfig /flushdns
ipconfig /registerdns
ipconfig /release
ipconfig /renew


15 commands you must know
https://www.makeuseof.com/tag/15-cmd-commands-every-windows-user-know/
