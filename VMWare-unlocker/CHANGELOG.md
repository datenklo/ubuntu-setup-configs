# Changes

All dates are UK format.
## 30/07/22 4.2.2
_drdonk_
* Re-worked README.md file
* Updated darwin.iso to version 12.0.6
* relock restarts Windows services unpatching fails
* Initial changes for 22H2 tech previews. New Windows service for auto-starting VMs needs to be stopped and started.
* Ensure using bash and fix dist folder creation in the source code build scripts fro Linux/macOS

## 03/06/22 4.2.1
_drdonk_:
* Missing message when removing ISOs in relock
* Updated darwin.iso to version 12.0.5

## 13/05/22 4.2.0
_drdonk:_
* Split unlocker.exe into 2 new files unlock.exe and relock.exe so can be directly executed on Windows without 
having to pass a parameter to install or uninstall
* Added Windows manifest to allow the executables to directly run as Administrator without using re-spawn code 
* Minimize false AV detection especially Windows Defender
* Added a new command to check the status of the patching called check.exe
* Fix to restarting vmware-tray.exe on Windows which had the wrong working directory

## 03/03/22 4.1.3
_drdonk:_
* Update VMware Tools to version 12.0.0

## 15/02/22 4.1.2

_drdonk:_
* Fix stopping/starting services on Windows due to service dependencies

## 26/01/22 4.1.1

_drdonk:_
* Fix copying of VMware tools ISO to the VMware installation folder
* Added a new troubleshooting page
* Updated copyright to 2022

## 09/12/21 4.1.0

Changed version to 4.1.0 due to the large number of changes to code submitted by boostchicken. 
Thanks to boostchicken for the fixes and improvements to the code.

_boostchicken:_
* Refactor to be more go like
* Fix vmware-shell-ext-thunker.exe preventing patching on windows
* Fixed header offset bug and binpack allocs
* Cleaned up logic regarding restoring backups or not
* Elevate permissions on Windows automatically

_drdonk:_
* Key press message changed to correct input of enter key
* Build macOS dumpsmc executable

## 06/12/21 4.0.0
* Initial release
