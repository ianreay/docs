.. _powershell:
Powershell
===============================================================================

Help
-------------------------------------------------------------------------------

Get-Command
* Lists all powershell commands

Get-Help <command>
* Returns help info for each command
  
Get-Member
* Returns functions that can be run on a certain object
* "something" | Get-Member will emit out all methods applicable to System.string.  
* gm - short alias

.Net
-------------------------------------------------------------------------------

New-Object
* Allows you to create new objects
** $rand = New-Object -TypeName System.Random -ArgumentList 42
** $rand.Next()

Inline c# code.
* Its possible to put inline c# chode into powershell scripts if you need the full power of .Net.

Drives
-------------------------------------------------------------------------------

Get-PSDrive

Remotable cmdlets
-------------------------------------------------------------------------------

Get-Help * -Parameter computername

* Test-Connection
* Test-WSMan

WMI
-------------------------------------------------------------------------------

Get-WmiObject -Class __Win32Provider | select name

* List wmi providers
