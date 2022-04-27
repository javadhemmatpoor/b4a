# Convert English Number To Persian Number

* function en2fa:

```basic4android
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

```b4a
entfa(123)
```

* exit

```log
    ۱۲۳
```

[hp](http://hemmatpoor.ir)
