# WindowsOnArm-X-Elite 
20241130
## Asus Vivobook S15 X-Elite

Developer Tools Setup

### Visual Studio 2022 Community Edition (Arm64)
- download from microsoft
- do not install version 2019
- not support .net framework 3.5 sdk
- not support .net core 3.1
- install component for rust
  - MSVC v143 - VS2022 C++ ARM build tools (Latest) 
  - MSVC v143 - VS2022 C++ ARM64/ARM64EC build tools (Latest)
  - Windows 11 SDK
  
### Visual Studio Code (Arm64)

### TortoiseSVN 1.14.8 (Arm64)
- [download](https://tortoisesvn.net/downloads.html)

### WinMerge 2.16.44 (Arm64)
- [download](https://winmerge.org/downloads/?lang=en)

### OpenVPN 2.6.12 (Arm64)
- [download](https://openvpn.net/community-downloads/)
- sophos client not able to run on arm, use OpenVPN client

### Rust (Arm64)
- [download](https://www.rust-lang.org/tools/install) RUSTUP-INIT.EXE (64-BIT)
- run the rustup-init.exe, follow the prompt instruction.

### Lapce (Arm64)
- clone from [github](https://github.com/lapce/lapce), compile it.
```sh
cargo install --path . --bin lapce --profile release-lto --locked
## will install to C:\Users\_YourUser_\.cargo\bin
```
### SSMS (x86)
### Git (x86)

### Zed
- tbc

### draw.io V24.7.17 (Arm64)

### mRemoteNG 1.76.20 (x86)
- [download](https://mremoteng.org)
  
