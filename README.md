rAthena-syntax-highlight
======================

Defined rAthena NPC scripting language for Notepad++.

## Keywords contents
 - NPC script commands.
 - Constants from db/const.txt


## How to add to Notepad++?
 - Open your Notepad++ and go to the Language > Define your language... > Import.
 - Use default styles in the Settings > Style Configurator > Select theme: Default.
 - Or you can download example style theme /themes/rAthenaWhite.xml and import it Settings < Import < Import style theme(s)....
 - Restart Notepad++ after changing language or styles.


## Make a new style theme or edit existing one:
 - Make a new theme by copying stylers.xml in ( %APPDATA%\notepad++ ) and rename it for your theme and edit it.
 - Save it in ( %APPDATA%\notepad++\themes ) folder.
 - Restart Notepad++ after edit.


## Auto-completion
 - Copy APIs/rathena.xml to Notepad++ installation folder APIs/rathena.
 - Open menu Settings > Preferences... > Auto-Completion tab, check "Enable auto-completion on each input".
 - Restart Notepad++.


## Sources:
 - [rAthena Script Commands](https://github.com/rathena/rathena/blob/1d88575f90b5f572cffba4a361f3028003008ffb/doc/script_commands.txt)
 - [rAthena Constants: db](https://github.com/rathena/rathena/blob/1d88575f90b5f572cffba4a361f3028003008ffb/db/const.txt)
 - [rAthena Constants: script_constants.hpp](https://github.com/rathena/rathena/blob/1d88575f90b5f572cffba4a361f3028003008ffb/src/map/script_constants.hpp)

## Groups of Keyword Lists
### 1st Group
Color: 0000FF
* All script commands except
  * mes, it has own group!
  * Flow control: if else switch case do while for
  * Most usage commands: next close close2 close3 menu select callsub callfunc

### 2nd Group
Color: 0080C0
* Variable with scope: @ . .@ \'

### 3rd Group
Color: FF8040
* Variable with scope: $ $@ # ##

### 4th Group
Color: FF0000
* Keywords using prefix for common labels and functions: On F_ S_ L_

### 5th Group
Color: 800040
* Flow control: if else switch case default do while for
* Most usage commands to make clear the block: next close close2 close3 end menu select callsub and callfunc

### 6th Group
Color: FF0080
* All constants that grouped by prefix identifiers
* Item Bonuses constants

### 7th Group
Color: FF0080
* All constants that are not grouped by prefix identifier
* Constants of NPC names (if only rAthena's script use `JT_` in script, this is not necessary)

### 8th Group
Color: FF0080
* `mes` script command

Happy editing.
