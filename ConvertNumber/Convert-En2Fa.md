# Convert English Number To Persian Number

* function en2fa:

```vb
Sub en2fa(a As String) As String
    ' تبدیل اعداد لاتین به فارسی
    Dim fa As String="۰۱۲۳۴۵۶۷۸۹"
    For la=0 To 9
        a=a.Replace(la,fa.SubString2(la,la+1))
    Next
    Return a
End Sub
```

* use:

```vb
entfa(123)
```

* exit

```vb
    ۱۲۳
```

[hp](http://hemmatpoor.ir)
