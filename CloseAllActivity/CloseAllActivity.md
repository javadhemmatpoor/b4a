# Close All Activity And Exit Application

* function CloseAllExit lib JavaObject:

```basic4android
Public Sub CloseAllExit
    Dim jo As JavaObject
    jo.InitializeContext
    jo.RunMethod("finishAffinity", Null)
End Sub
```

* use:

```b4a
CloseAllExit
```

[hp](http://hemmatpoor.ir)