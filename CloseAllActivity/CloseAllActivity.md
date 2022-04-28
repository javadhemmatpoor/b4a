# Close All Activity And Exit Application

* function CloseAllExit lib JavaObject:

```vb
Public Sub CloseAllExit
    Dim jo As JavaObject
    jo.InitializeContext
    jo.RunMethod("finishAffinity", Null)
End Sub
```

* use:

```vb
CloseAllExit
```

[hp](http://hemmatpoor.ir)