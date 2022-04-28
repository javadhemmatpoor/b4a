# Share Text

* function Share Text Intent:

```vb
Sub ShareTxt(body as string,title as string)
    Dim x As Intent
    x.Initialize(x.ACTION_SEND,"")
    x.SetType("text/plain")
    x.PutExtra("android.intent.extra.TEXT", body)
    x.WrapAsIntentChooser(title)
    StartActivity(x)
End Sub
```

* use:

```vb
ShareTxt("Mohtava","Subject")
```

[hp](http://hemmatpoor.ir)
