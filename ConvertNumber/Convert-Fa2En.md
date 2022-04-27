# Convert Persian Number To English Number

* function fa2en:

```basic4android
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

```b4a
fa2en(۱۲۳)
```

* exit

```log
    123
```

[hp](http://hemmatpoor.ir)
