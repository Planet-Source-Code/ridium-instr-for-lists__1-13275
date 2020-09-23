<div align="center">

## InStr for lists


</div>

### Description

will search a listbox's contents for a string returning a True if the string exists and a False if it dosent
 
### More Info
 
lst = The Listbox

zString = The string to search the list for

True or False depending on if the string was found


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Ridium](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/ridium.md)
**Level**          |Beginner
**User Rating**    |4.5 (18 globes from 4 users)
**Compatibility**  |VB 3\.0, VB 4\.0 \(16\-bit\), VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0
**Category**       |[String Manipulation](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/string-manipulation__1-5.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/ridium-instr-for-lists__1-13275/archive/master.zip)





### Source Code

```
Function ListIsIn(lst As ListBox, zString As String) As Boolean
On Error Resume Next
For i = 0 To lst.ListCount
  If lst.List(i) = zString Then ListIsIn = True: GoTo grr
Next i
ListIsIn = False
grr:
End Function
```

