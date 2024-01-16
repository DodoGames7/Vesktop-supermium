# Vesktop (with Supermium Electron)
Re-packaged version of Vencord's desktop for older windows versions (example: 7 - 8.1).

# disclaimer
This is not intended to keep using end-of-life Windows versions. 

You're still highly recommended to use a supported one such as Windows 10 or 11 (or even try Linux?). Using them can have security issues and i wouldn't recommend having a daily driver with those releases. This repo is not affiliated with the regular Vesktop or Vencord devs at all and support for it should not be requested in Vencord's server.

# Supported versions
Because Supermium Electron fork intends to support EOL releases of windows, the Re-packaged application can run on the following:
* Windows 7
* Windows 8.1 (and prolly 8.0)

At the moment, earlier versions aren't supported without modifications. Those include:
* Windows Vista Service pack 3 (with extended kernel)
* Windows XP Service pack 3 (64-bit professional with one-core API)

# Re-producing yourself
It is possible to make Vesktop compatible with older Windows versions using supermium electron's archive:

### Configuring Vesktop to use Supermium Electron
1. Download the Supermium Electron zip from [Releases](https://github.com/win32ss/supermium-electron/releases/download/v28-testing)
2. Download the latest Vesktop Windows zip from [here](https://github.com/Vencord/Vesktop/releases).
3. Extract both zip files
4. Delete the entire resources folder from Supermium Electron folder
5. Move the resources folder from Vesktop folder to Supermium Electron folder
6. Run `electron.exe`

 You're done after that. Vesktop should now run on old Windows versions!

# Blank window
There's a chance that opening the Re-packaged application can have a empty window. This can be bypassed by applying a `settings.json` file to Vencord Desktop's appData folder:

### On dual-boot install
1. On a regular windows supported install with Vesktop installed, Press the Windows key + R and enter `%APPDATA%` respectively
2. Enter into the `VencordDesktop` directory. You will notice by default that there's another folder with the same name, enter into the folder as well
3. Copy the `settings.json` file or save it else where so that you can use it again
4. Repeat the same steps on another version of windows and place your `settings.json` file inside of the same place where you obtained the `settings.json` file from on another windows install
5. You're all set, the application should now launch normally.

If you want to just directly have a copy of an example `settings.json` file then take a look at [Releases](https://github.com/DodoGames7/Vesktop-supermium/releases) tab.


### On Single install
You can obtain a pre-ready `settings.json` file from [Releases](https://github.com/DodoGames7/Vesktop-supermium/releases).



