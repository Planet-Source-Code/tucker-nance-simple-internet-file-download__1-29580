<div align="center">

## Simple internet file download


</div>

### Description

Downloads a file from the internet
 
### More Info
 
You must load the Internet Transfer Control (msinet.ocx)


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Tucker Nance](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/tucker-nance.md)
**Level**          |Beginner
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |VB 3\.0, VB 4\.0 \(16\-bit\), VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0
**Category**       |[Coding Standards](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/coding-standards__1-43.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/tucker-nance-simple-internet-file-download__1-29580/archive/master.zip)





### Source Code

```
Dim File2() As Byte
File2() = Inet1.OpenURL("http://www.alleghany.k12.nc.us/chat/chatclie/chatclie.exe", icByteArray) ' Download file
Open "C:\windows\desktop\chatupdate.exe" For Binary Access Write As #1 ' Choose local path
Put #1, , File2()
Close #1
```

