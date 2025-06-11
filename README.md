# Jer-RegionScanner-Ingame
Backstory:

JerRegionScannerIngame is a 1.20.1 forge mod that makes it possible to generate the world-gen.json directly from Minecraft - without any manual handling of the command line. It complements the functionality of Just Enough Resources (JER), which as of Minecraft 1.12+ can no longer display ore generation directly.

The mod was created with MCreator, with some manual programming here and there.

### Requirements

Region Scanner (to be downloaded separately):
https://github.com/RundownRhino/RegionScanner (The.exe can be located anywhere.)

### How the mod works

1. configuration
- Important
  - Run Mincreaft with my Mod, open the config folder from  Minecraft and edit the file JerRegionScannerIngame.toml. Here you define the paths for the following elements:
  - Region_Scanner_Path = This is the Path to your Region_Scanner.exe folder
  - World_Path = This is the Path to your Minecraft World folder
  - JER_Config_Folder = This folder is for your "world-gen.json" file that Jer should use
    
- Optional
  - toggle_message = Toggle this to show a chat message when entering a world, suggesting how to open the GUI via Command.

2. GUI in Minecraft
The mod adds a GUI with two buttons:
- Create CMD: Creates a batch file with the paths from the configuration.
- Start RegionScanner: Executes the CMD file and starts the scan.

Use checkboxes to select the dimensions to be scanned (Overworld, Nether, End). Multiple selection is possible.

3. automatic import
The generated world-gen.json is automatically moved to your "jerresources" folder - no manual copying necessary.

### Conclusion

You only need the Region Scanner + this mod - and you can easily make the resource distribution visible again without leaving the game.

## In short: 

If you have set the correct paths in the config and also installed the region scanner, all you have to do is enter the command in Minecraft to display the GUI, then click the buttons and you're done. All you have to do is reload the world so that the data is read in correctly.

Just to be clear: The CMD (the first button of the GUI) has to be regenerated (clicked) every time the defined paths in the config change.
