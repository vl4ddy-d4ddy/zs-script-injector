# ZERO Sievert Script Injector (ZSSI)
ZSSI is a mod for ZERO Sievert that allows user to inject and run custom .dll files, these files are stored in the games directory under a folder called "mods". When the main menu is created, the mod runs a function that looks for all .dll files, and executes a function in them under the name "main". I have not tested the plugin fully yet so feel free to make your own .dll mods for this wonderful game.

### Installation
Installing ZSSI is a little different to the mods that change .json file. The releases will include a file called "DeltaPatcher.exe" and "ZSSI.xdelta". To install, open up DeltaPatcher, for the original file, put the location of the games data.win file, and for the XDelta patch, put the location of "ZSSI.xdelta". Then just click "Apply Patch" and you're good to go! No need to use Mod Organiser 2 or overwriting silly .json files!

### For Developers
Making a plugin/mod is simple, you make a new Visual Studio project for a .dll (Dynamic Link Library). Add a function called "main", **all lowercase**, and write the code you'd like to execute inside main. Once completed, build the .dll and put it in the "mods" folder in the games directory.
