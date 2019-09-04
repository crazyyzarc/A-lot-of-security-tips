# Mit welchem Installer erstellt?

## Windows [needed strings.exe*]
> strings.exe <mysetup.exe> | findstr /i /r "inno installshield nsis wise"


## Linux [strings included]
> strings <mysetup.exe> | grep -i -E "(inno|nsis|installshield|wise)"

*Quelle: https://docs.microsoft.com/en-us/sysinternals/downloads/strings [Windows only]
