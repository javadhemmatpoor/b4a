# Change Fonts All Label

* function Change Font Label:

```basic4android
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

```b4a
ChangeFont_Label
```

[hp](http://hemmatpoor.ir)