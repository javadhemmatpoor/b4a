# Convert Persian Number To English Number

* function fa2en:

```vb
Sub fa2en(a As String) As String
    ' تبدیل اعداد فارسی به لاتین
    Dim fa As String="۰۱۲۳۴۵۶۷۸۹"
    For la=0 To 9
        a=a.Replace(fa.SubString2(la,la+1),la)
    Next
    Return a
End Sub
```

* use:

```vb
fa2en(۱۲۳)
```

* exit

```vb
    123
```

[hp](http://hemmatpoor.ir)
