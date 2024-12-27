## Markdown
### [Markdown Preview Language Server](https://github.com/euclio/mdpls)

https://github.com/helix-editor/helix/issues/2824

#### Install
```bash
cargo install --git https://github.com/euclio/mdpls
# C:\Users\cmwong\.cargo\bin\mdpls.exe
```
#### Config
```toml
# C:\Users\cmwong\AppData\Roaming\helix\languages.toml
[[language]]
name = "markdown"
language-servers = ["mdpls"]

[language-server.mdpls]
command = "mdpls"
config = { markdown.preview.auto = true, markdown.preview.browser = "C:\\Program Files\\Mozilla Firefox\\firefox.exe" }
```


```bash
## mklink c:\Windows\System32\firefox.exe "C:\Program Files\Mozilla Firefox\firefox.exe"
```