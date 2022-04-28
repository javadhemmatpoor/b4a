# Separate 3 digits 3 digits

* function ToCurrencyFormat:

```vb

Sub ToCurrencyFormat(d As Double) As String
    ' تابع جداکردن اعداد 3 رقم 3 رقم
    Dim s As String = NumberFormat2(d, 1, 3, 0, True)
    Return s.Replace(".", ",")
End Sub
```

* use:

```vb
ToCurrencyFormat(130000000)
```

* exit

```log
    130,000,000
```

* use EditText:

```edittext
Sub EditText1_TextChanged (Old As String, New As String)
    ' نحوه استفاده در ادیت تکست
  
    If New.Trim="" Then Return
  
    Dim s As String = New.Replace(",","")
    s = ToCurrencyFormat(s)
  
    If s <> EditText1.Text Then
        EditText1.Text = s
        EditText1.SelectionStart = EditText1.Text.Length
        End If
End Sub
```

[hp](http://hemmatpoor.ir)
