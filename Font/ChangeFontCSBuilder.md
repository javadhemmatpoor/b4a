# Change Fonts All

* function CSBuilder:

```basic4android
Public Sub CS(text As String) As CSBuilder
    ' تغییر فونت اجزای برنامه
    Dim c As CSBuilder
    c.Initialize.Typeface(Typeface.LoadFromAssets("font-name.ttf")).Append(text).PopAll
    Return c
End Sub
```

* use:

```b4a
toastmessage(cs("testFont"),False)
```

[hp](http://hemmatpoor.ir)
