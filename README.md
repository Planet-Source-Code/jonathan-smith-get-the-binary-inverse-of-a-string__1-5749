<div align="center">

## Get the binary inverse of a string


</div>

### Description

This code is the equivalence of the bitwise complement C opertator (~), except this only works on strings. I got tired of not having this capability, so I wrote it =)
 
### More Info
 
any string

the bitwise inverse of the string

works ONLY on strings


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Jonathan Smith](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/jonathan-smith.md)
**Level**          |Intermediate
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |VB 3\.0, VB 4\.0 \(16\-bit\), VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0, VB Script, ASP \(Active Server Pages\) 
**Category**       |[String Manipulation](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/string-manipulation__1-5.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/jonathan-smith-get-the-binary-inverse-of-a-string__1-5749/archive/master.zip)





### Source Code

```
Public Function BinaryInverse(ByVal szData As String)
  Dim szRet As String
  szRet = Space$(Len(szData))
  For i = 1 To Len(szData)
    Mid(szRet, i, 1) = Chr$(255 - Asc(Mid(szData, i, 1)))
  Next i
  BinaryInverse = szRet
End Function
```

