![thumbnail](https://github.com/OpenToontownTools/web/blob/master/assets/openrtm_thumb.png)

# Open Robot Toon Manager (RTM)
## About RobotToon ##
RobotToon was a development tool for Disney's Toontown Online artists to create scenes for backgrounds to be used as wallpapers, blog posts, and various graphic design related assets. OpenRTM is an open source project aimed to update the RTM to be compatible with the latest verisons of Panda3D, Python 3, and with feature improvements.

## Development Progress
* This project is in very early development and is pretty unusable. Feel free to contribute to the project.

## Requirements
### ***IMPORTANT***
* **You will need the [Toontown Realms Panda3D SDK](https://toontownrealms.com/dev/Panda3D-TTRMDev-1.11.0-py3.6-x64.exe)**
* Toontown phase files that include all the dna files. [These](https://github.com/open-toontown/resources) work fine. ***Toontown Rewritten's phase files do NOT contain .dna files since they use a completely different format, so you need to use them from elsewhere. Open-Toontown's resources are the closest to Toontown Online's that you can get, while also being completely updated and compatible with Panda3D 1.10.x.***
    * These phase files go in the ROOT directory of the editor

## Credits
* [Disyer](https://github.com/darktohka/) - Project Lead | Developer
* [Loonatic](https://github.com/loonaticx/) - Project Lead | Developer
* [drewcification](https://github.com/drewc5131) - Open Toontown Tools Project Lead | Developer
* [Any other contributors are listed on the side](https://github.com/OpenToontownTools/OpenRTM/graphs/contributors)

# FAQ

### Some of my props are using textures as if they were in a different playground?
* This is OK. This is just because you have support for more than 1 playground loaded. This is only visible in the editor, but I recommend you only load the zone you are working on.

### I did the setup properly, but the editor just closes on startup with no error message, how do I fix?
* If you are downloading my redistributed copy of Panda from above, this may be an issue of having multiple installations of panda, and an incorrect one being targeted. Try one or both of the following:
    * Edit the registry
        * Open RegEdit
        * Navigate to `Computer\HKEY_CURRENT_USER\SOFTWARE\Python\PythonCore\3.9\InstallPath`
        * Change (Default)'s value to `C:\Panda3D-1.11.0-py39-x64\python`
        * Change ExecutablePath's value to `C:\Panda3D-1.11.0-py39-x64\python\python.exe`
        * Save, and if that does not work try restarting your PC, or doing option #2
    * Remove all other versions of Panda3D.
