# Run Application Intent

* function run app instagram:

```vb
Sub RunApp_Instagram
    Private i As Intent
    i.Initialize(i.ACTION_MAIN,"")
    i.SetComponent("com.instagram.android")
    StartActivity(i)
End Sub
```

* use:

```vb
RunApp_Instagram
```

[hp](http://hemmatpoor.ir)
