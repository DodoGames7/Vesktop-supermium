# Vesktop (with Supermium Electron)
Re-packaged version of Vencord's desktop for older windows versions (example: 7 - 8.1).

# disclaimer
This is not intended to keep using end-of-life Windows versions. 

You're still highly recommended to use a supported one such as Windows 10 or 11 (or even try Linux?). Using them can have security issues and i wouldn't recommend having a daily driver with those releases. This repo is not affiliated with the regular Vesktop or Vencord devs at all and support for it should not be requested in Vencord's official server.

# Supported versions
Because Supermium Electron fork intends to support EOL releases of windows, the Re-packaged application can run on the following:
* Windows 7
* Windows 8.1 (and prolly 8.0)

At the moment, earlier versions aren't supported without modifications. Those include:
* Windows Vista Service pack 2 (64-bit with Extended Kernel)
* Windows XP 64-bit Edition (AMD64 architecture) (With SP3 including One-Core-API)

They also aren't tested so there's no confirmation from me on whether or not the Re-packaged application will work there

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
There's a chance that opening the Re-packaged application can have a empty/invisible window for first launch window. This can be bypassed by applying a two files to Vencord Desktop's appData folder:

### On dual-boot install
This method is for people who dual boot Windows 10/11 with EOL windows versions like 7

1. On a regular windows supported install with Vesktop installed, Press the Windows key + R and enter `%APPDATA%` respectively
2. Enter into the `vesktop` directory
3. Copy the `settings.json` and `state.json` file to else somewhere so that you can use it again (such as a USB)
4. Repeat the same steps on another version of windows and place both of the files inside of the same directory where you obtained the files from the other windows install
5. You're all set, the application should now launch normally.




