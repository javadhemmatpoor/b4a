# Detect Phone Language

* function GetLanguage:

```basic4android
Sub GetLanguage As String
    ' تابع تشخیص زبان گوشی
    Dim r As Reflector
    r.Target = r.RunStaticMethod("java.util.Locale", "getDefault", Null, Null)
    Return r.RunMethod("getDisplayName")
End Sub
```

* use:

```b4a
log(GetLanguage)
```

* exit

```log
    English (United States)
```

[hp](http://hemmatpoor.ir)
