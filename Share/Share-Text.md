# Share Text

* function Share Text Intent:

```basic4android
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

```b4a
ShareTxt("Mohtava","Subject")
```

[hp](http://hemmatpoor.ir)
