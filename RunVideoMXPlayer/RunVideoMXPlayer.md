# Open Video Play MXPlayer

* function open Video MXPlayer:

```vb
Sub MXPlayer(VideoAddress As String)
    Dim i As Intent
    i.Initialize(i.ACTION_VIEW,VideoAddress)
    i.SetComponent("com.mxtech.videoplayer.ad/.ActivityScreen")
    StartActivity(i)
End Sub
```

* use:

```vb
' Offline:
MXPlayer(File.Combine(File.DirRootExternal,"BasicLearn.mp4"))

' Online:
MXPlayer("https://basiclearn.ir/Videos/Example.mp4")
```

[hp](http://hemmatpoor.ir)
