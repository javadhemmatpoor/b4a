# Detect Phone Language

* function GetLanguage:

```vb
Sub GetLanguage As String
    ' تابع تشخیص زبان گوشی
    Dim r As Reflector
    r.Target = r.RunStaticMethod("java.util.Locale", "getDefault", Null, Null)
    Return r.RunMethod("getDisplayName")
End Sub
```

* use:

```vb
log(GetLanguage)
```

* exit

```vb
    English (United States)
```

[hp](http://hemmatpoor.ir)
