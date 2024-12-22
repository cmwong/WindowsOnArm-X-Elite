## Helix

### installation
```bash
winget install Helix.Helix
# x64
```

### Space Mode
press `space` key to enter space mode

f - Open file picker
F - Open file picker at current working directory

#### to navigate file in file picker
```bash
# Tab,       Crtl-n - next entry
# Shift Tab, Ctrl-p - previous entry
```

### Goto Mode
press `g` in normal mode

### connfigure typescript lsp
```bash
nvm list
# output
#    20.18.1
#  * 18.20.5 (Currently using 64-bit executable)
#    16.20.2
#    14.21.3

hx --health typescript
# output
# Configured language servers:
#  ✘ typescript-language-server: 'typescript-language-server' not found in $PATH
# Configured debug adapter: None
# Configured formatter: None
# Highlight queries: ✓
# Textobject queries: ✓
# Indent queries: ✓

# install typescript lsp for node 18.20.5
npm install -g typescript-language-server typescript

# need to install for each of the version of node
```