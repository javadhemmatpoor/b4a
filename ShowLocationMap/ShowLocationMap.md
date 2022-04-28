# Show Location Google Map

* function:

```vb
Sub ShowLocation(number1 As Double, number2 As Double)
    Try
        Dim GMP As Intent
        GMP.Initialize(GMP.ACTION_VIEW,"geo:0,0?q="& number1 & ","& number2 &"")
        StartActivity(GMP)
    Catch
        ToastMessageShow("برنامه Google Maps در گوشی شما نصب نیست !",False)
    End Try
End Sub
```

* use:

```vb
ShowLocation(36.419503982415655,54.96498584747315)
```

[hp](http://hemmatpoor.ir)
