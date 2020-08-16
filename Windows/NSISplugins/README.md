# NSIS Plugins
A NSIS plugin is a way of extending installer’s functionality by adding new functions.

NSIS plugins can be donwloaded from - https://nsis.sourceforge.io/Category:Plugins or by searching for it on [NSIS Wiki](https://nsis.sourceforge.io/Main_Page)

NSIS plugins consist of one mandatory file (with the extension *.dll*) and usually a header file (with the extension *.nsh*).

NSIS  searches  for  plugins  in  the `Plugins` folder  under  the  NSIS  install  directory and lists all of their available functions. `!addplugindir` command can be used to tell NSIS to search in other directories too.

Steps to install NSIS plugins -
* After downloading the plugin, unpack it. It may contains various files along with the `.dll` file and/or `.nsh` file.
* Then  the  `.dll`  files  must  be  put  into  the  `NSIS/Plugins[/platform]` subfolder and the `.nsh` file into the `NSIS/Include` subfolder.
* Plugins with extension `.nsh` can be placed in the same dirctory as the NSIS script in which the plugin is to be used and can be included using the command `!include "plugin.nsh"`.

> `NSIS/` - refers to the location where NSIS is installed on the system.
