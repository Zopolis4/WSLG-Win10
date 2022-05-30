# WSLG-Win10

Ongoing research with the end goal of being easily able to use WSLg on regular Windows 10 builds without admin (beyond the inital admin required for the WSL2 install). 

Huge thanks to https://github.com/Biswa96/initrdg and https://github.com/Biswa96/WslReverse.

## Extracting the .msi
Currently, the best way to extract the `wsl_graphics_support_x64.msi` file is through the following command:
```
msiexec /a wsl_graphics_support_x64.msi /qf TARGETDIR=full\path\to\dir
```
This works on any build of Windows 10 and does not require admin.

This should also work for `wsl_graphics_support_arm64.msi`, although it seems that you need to be on an arm64 machine.
