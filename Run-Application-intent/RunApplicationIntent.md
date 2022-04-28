# Run Application Intent

* function run app instagram:

```basic4android
Sub RunApp_Instagram
    Private i As Intent
    i.Initialize(i.ACTION_MAIN,"")
    i.SetComponent("com.instagram.android")
    StartActivity(i)
End Sub
```

* use:

```b4a
RunApp_Instagram
```

[hp](http://hemmatpoor.ir)
