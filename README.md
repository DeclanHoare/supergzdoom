supergzdoom is an extremely simple WAD selector for gzdoom written in Bash using Zenity.

##Setup
IWADs go in ~/.config/supergzdoom/iwads, and PWADs for an IWAD go in ~/.config/supergzdoom/pwads/(IWAD NAME).
(The path can be configured with a variable at the top of the file, as can the executable for gzdoom.)

##Operation
Upon running supergzdoom, you can choose an IWAD and any PWADs you would like to use with it.
It will then launch gzdoom with the correct parameters and change the save directory based on your selections;
if you chose no PWADs, the save directory will be set to ~/.config/supergzdoom/saves/(PWAD NAME), and if you
did choose some, the save directory will be set based on the md5sum of the name of your IWAD and all chosen PWADs.
This is, obviously, to ensure that no save files will be overwritten when playing different games.
