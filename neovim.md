## NeoVim
[reference](https://blog.nikfp.com/how-to-install-and-set-up-neovim-on-windows)



### Install
```bash
# install ripgrep, command rg
winget install BurntSushi.ripgrep.MSVC
# or winget install 'ripgrep msvc'

winget install Neovim.Neovim
# neovim is x86

# this is powershell (not Windows Powershell)
# winget install microsoft.powershell
# hang when installing, do the next step, download from microsoft
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
```bash
# c:\Users\_user_\AppData\Local\nvim
# - lua
#   - my_user
#       - core
#           - init.lua
#           - keymaps.lua
#           - options.lua
#       - plugins
#           - init.lua
#           - nvim-tree.lua
#           - treesitter.lua_x
#       - lazy.lua
#   - init.lua
```

### nvim-tree - A File Explorer For Neovim Written In Lua
Open the tree: `:NvimTreeOpen`
Show the mappings: `g?`
```bash
# <leader>ee - Toggle file explorer
# <leader>ef - Toggle file explorer on current file
# <leader>ec - Collapse file explorer
# <leader>er - Refresh file explorer
# <C-w>w    - switch between explorer and editor
```

- nvim-treesitter is not working 
