# Change Fonts All

* function CSBuilder:

```vb
Public Sub CS(text As String) As CSBuilder
    ' تغییر فونت اجزای برنامه
    Dim c As CSBuilder
    c.Initialize.Typeface(Typeface.LoadFromAssets("font-name.ttf")).Append(text).PopAll
    Return c
End Sub
```

* use:

```vb
toastmessage(cs("testFont"),False)
```

[hp](http://hemmatpoor.ir)
