# Notepad++ als Standard Windows Editor / Notepad++ as standard text editor

Gemäß der Anleitung von deskmodder ist es möglich den Standard Editor unter Windows durch Notepad++ zu ersetzen.

Link: https://www.deskmodder.de/blog/2018/10/22/notepad-7-5-9-kann-nun-den-windows-editor-als-standard-ersetzen/

```diff
! Diese Konfiguration erfordert Notepad++ Version 7.5.9+
```

</br>

## 32-Bit
> reg add "HKLM\Software\Microsoft\Windows NT\CurrentVersion\Image File Execution Options\notepad.exe" /v "Debugger" /t REG_SZ /d "\"%ProgramFiles(x86)%\Notepad++\notepad++.exe\" -notepadStyleCmdline -z" /f

## 64-Bit
> reg add "HKLM\Software\Microsoft\Windows NT\CurrentVersion\Image File Execution Options\notepad.exe" /v "Debugger" /t REG_SZ /d "\"%ProgramFiles%\Notepad++\notepad++.exe\" -notepadStyleCmdline -z" /f

## Entfernen / Remove
> reg delete "HKLM\Software\Microsoft\Windows NT\CurrentVersion\Image File Execution Options\notepad.exe" /v "Debugger" /f
