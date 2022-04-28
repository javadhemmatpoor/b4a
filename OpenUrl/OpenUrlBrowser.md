# Open URL Browser Phone

* function open url browser:

```basic4android
Sub OpenUrl(Url As String)
    Private i As Intent
    i.Initialize(i.ACTION_VIEW,Url)
    StartActivity(i)
End Sub
```

* use:

```b4a
OpenUrl("https://google.com")
```

[hp](http://hemmatpoor.ir)
