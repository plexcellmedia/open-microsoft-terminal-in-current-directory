# Microsoft Terminal: Open In Current Directory

### Installation
- Install Microsoft Terminal from Microsoft Store.
- Create `wt.reg` file, paste code below and replace `USERNAME` with your current username.
```sh
Windows Registry Editor Version 5.00

[HKEY_CLASSES_ROOT\Directory\Background\shell\wt]
@="Open Terminal Here"

[HKEY_CLASSES_ROOT\Directory\Background\shell\wt\command]
@="C:\\Users\\USERNAME\\AppData\\Local\\Microsoft\\WindowsApps\\wt.exe"
```
- Add `wt.reg` to registry
- Open terminal settings panel

![Settings](https://i.imgur.com/Mg5gz2x.png)

- Add line below to each profile, to make terminal open in current directory
```sh
"startingDirectory": "."
```