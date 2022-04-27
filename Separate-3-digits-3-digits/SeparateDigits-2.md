# Separate 3 digits 3 digits

* function ToCurrencyFormat:

```basic4android
Sub CommaNumberSplit (Txt As String) As String
    ' تابع جداکردن اعداد 3 رقم 3 رقم
    Dim Str = Txt As String,counter = 0 As Int
    For i = Str.Length-1 To 0 Step -1
        If IsNumber(Str.CharAt(i)) Then
            If counter < 2 Then
                counter = counter + 1
            Else if counter = 2 And i <> 0 Then
                Dim st1,st2 As String
                st1 = Str.SubString2(0,i)
                st2 = Str.SubString2(i,Str.Length)
                Str = st1 & "," & st2
                counter = 0
            End If
        End If
    Next
    Return Str
End Sub
```

* use:

```b4a
ToCurrencyFormat(130000000)
```

* exit

```log
    130,000,000
```

[hp](http://hemmatpoor.ir)
