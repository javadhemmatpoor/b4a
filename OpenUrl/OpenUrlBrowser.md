# Open URL Browser Phone

* function open url browser:

```vb
Sub OpenUrl(Url As String)
    Private i As Intent
    i.Initialize(i.ACTION_VIEW,Url)
    StartActivity(i)
End Sub
```

* use:

```vb
OpenUrl("https://google.com")
```

[hp](http://hemmatpoor.ir)
