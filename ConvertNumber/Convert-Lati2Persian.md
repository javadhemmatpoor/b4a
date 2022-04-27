# Convert English Number To Persian Number

* function PersianNumbers use replace Convert:

```basic4android
Public Sub PersianNumbers(Text As String) As String
    Dim s As String = Text
    s = s.Replace("0","۰")
    s = s.Replace("1","۱")
    s = s.Replace("2","۲")
    s = s.Replace("3","۳")
    s = s.Replace("4","۴")
    s = s.Replace("5","۵")
    s = s.Replace("6","۶")
    s = s.Replace("7","۷")
    s = s.Replace("8","۸")
    s = s.Replace("9","۹")

    Return s
End Sub
```

* use:

```b4a
PersianNumbers(123)
```

* exit

```log
    ۱۲۳
```

[hp](http://hemmatpoor.ir)
