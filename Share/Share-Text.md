# Share Text

* function Share Text Intent:

```basic4android
Sub ShareTxt
    Dim x As Intent
    x.Initialize(x.ACTION_SEND,"")
    x.SetType("text/plain")
    x.PutExtra("android.intent.extra.TEXT", "متن مورد نظر شما !")
    x.WrapAsIntentChooser("اشتراک گذاری متن")
    StartActivity(x)
End Sub
```

* use:

```b4a
ShareTxt
```

[hp](http://hemmatpoor.ir)
