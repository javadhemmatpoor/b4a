# Check Install Appliction

* function Check Install Appliction:

```vb
Sub CheckInstall(pakageName As String)
    Dim pm As PackageManager ,i As Intent
    i = pm.GetApplicationIntent(pakageName)
    If i.IsInitialized Then
        ToastMessageShow("برنامه نصب شده است !",True)
    Else
        ToastMessageShow("برنامه نصب نیست !",True)
    End If
End Sub
```

* use:

```vb
CheckInstall("pakage.name.app")
```

[hp](http://hemmatpoor.ir)