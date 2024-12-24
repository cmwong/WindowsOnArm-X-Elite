## Build Helix for native Windows Arm64

[download release 24.07](https://github.com/helix-editor/helix/releases/tag/24.07)
[build from source](https://docs.helix-editor.com/building-from-source.html)
[reference](https://github.com/helix-editor/helix/discussions/5490`)

```bash
setx HELIX_RUNTIME "C:\github_project\helix-24.07\runtime"
# need to restart terminal
```

```bash
# winget is install the x86_64 in
# C:\Users\cmwong\AppData\Local\Microsoft\WinGet\Packages\Helix.Helix_Microsoft.Winget.Source_8wekyb3d8bbwe\helix-24.07-x86_64-windows
# winget had set the above path to user PATH
# the runtime path is under helix-24.07-x86_64-windows
#
# folder structure 
# helix-24.07-x86_64-windows
#   \contrib
#   \runtime
#   hx.exe 
#   LICENSE
#   README.md


# C:\github_project\helix-24.07>echo %USERPROFILE%
# C:\Users\cmwong

# C:\github_project\helix-24.07>echo %APPDATA%
# C:\Users\cmwong\AppData\Roaming
```

### How should i place my helix Arm64 build?
```bash
# uninstall x86_64 helix
winget uninstall Helix.Helix
```

```bash
# cargo install --path helix-term --locked
# will place hx.exe in C:\Users\cmwong\.cargo\bin
# i don't want helix in cargo folder
#
# build helix
cargo build --profile opt --locked 

# from the source
# copy target\opt\hx.exe to C:\Program Files\helix 
# copy runtime folder to C:\Program Files\helix\runtime
#
# C:\Program Files\helix
#   \runtime
#       \grammer
#       \queries
#       \themes
#   hx.exe
#
# add C:\Program Files\helix to user PATH
#
# config file is in this folder
# C:\Users\cmwong\AppData\Roaming\helix
#
# log file in this folder
# C:\Users\cmwong\AppData\Local\helix

# run as administrator
robocopy target\opt "C:\Program Files\helix" hx.exe
# do not copy the sources folder
robocopy runtime "C:\Program Files\helix\runtime" /S /XD sources

```
### delete HELIX_RUNTIME
Setting -> System -> About -> Advanced system settings
Environment Variables -> User variables for xx
Delete HELIX_RUNTIME


