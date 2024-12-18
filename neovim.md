## NeoVim
[reference](https://blog.nikfp.com/how-to-install-and-set-up-neovim-on-windows)



### Install
```bash
# install ripgrep, command rg
winget install BurntSushi.ripgrep.MSVC
# or winget install 'ripgrep msvc'

winget install Neovim.Neovim

# this is powershell (not Windows Powershell)
# winget install microsoft.powershell
# hang when installing
```
[download powershell arm64 from microsoft](https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell-on-windows?view=powershell-7.4#msi)

### download Nerd font
[download MesloLG Nerd Font](https://www.nerdfonts.com/font-downloads) 
- extract it
- select all the fonts file, right click, install for all users.

### configure terminal to use Powershell
- Startup -> Default profile, change to "Powershell"

### configure terminal to use the Nerd Font
- open the setting
- Profile -> Defaults -> Appearance --> Font Face
- change to MesloLGS Nerd Font Mono

```bash
# linux ~/.config/nvim
# windows ~\AppData\Local\nvim

# linux ~/.local/share/nvim
# windows ~\AppData\Local\nvim-data
```

### [Configure NeoVim](https://www.josean.com/posts/how-to-setup-neovim-2024)

