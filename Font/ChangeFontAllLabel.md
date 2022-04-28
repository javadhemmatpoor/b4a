# Change Fonts All Label

* function Change Font Label:

```vb
Public Sub ChangeFont_Label
    For Each v As View In Activity.GetAllViewsRecursive
        If v Is Label Then
            Dim lb As Label = v
            lb.Typeface = Typeface.LoadFromAssets("font.ttf")
        End If
    Next
End Sub
```

* use:

```vb
ChangeFont_Label
```

[hp](http://hemmatpoor.ir)