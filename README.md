﻿# G-Code Language Extension

## Installation - Visual Studio Market Place

https://marketplace.visualstudio.com/items?itemName=gojimmypi.gojimmypi-gcode-language-extension

## Installation - Manual install with source code 

Find the location of your `VSIXInstaller.exe`, typpically in `.\Common7\IDE\` of Developer Command Prompt. Shown is an example of VS2017 Enterprise:

```
c:
cd \workspace
git clone https://github.com/gojimmypi/GcodeLanguageExtension.git
cd GcodeLanguageExtension
msbuild GcodeLanguage.csproj
"C:\Program Files (x86)\Microsoft Visual Studio\2017\Enterprise\Common7\IDE\VSIXInstaller.exe"  C:\workspace\GcodeLanguageExtension\bin\Release\GcodeLanguage.vsix
```

## Removal

```
"C:\Program Files (x86)\Microsoft Visual Studio\2017\Enterprise\Common7\IDE\VSIXInstaller.exe" /uninstall:TBD TODO
```

## Testing

Open the project and press `F5` to launch an experimental versional of Visual Studio.

## Modifications

TODO

## Case Sensitivity
There seems to be a disagreement between various sources as to whether G-Code is case senstiive. According to  RS274/NGC Interpreter - Version 3, page 23:

"Input is case insensitive, except in comments, i.e., any letter outside a comment may be in upper
or lower case without changing the meaning of a line."

## Resources
* [The NIST RS274NGC Interpreter - Version 3](https://ws680.nist.gov/publication/get_pdf.cfm?pub_id=823374)
* [wikipedia - G-Codes](https://en.wikipedia.org/wiki/G-code)
* [linuxcnc G-Code Quick Reference](http://linuxcnc.org/docs/html/gcode.html)
* [linuxcnc - M-Codes](http://linuxcnc.org/docs/html/gcode/m-code.html#mcode:m2-m30)
* [linuxcnc - G-Codes](http://linuxcnc.org/docs/html/gcode/overview.html)
* [linuxcnc - O-Codes](http://linuxcnc.org/docs/html/gcode/o-code.html)