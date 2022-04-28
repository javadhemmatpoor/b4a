# Random Number

* function Rnd:

استفاده از تابع پیش فرض نرم افزار

ایجاد عدد تصادفی بین 0 تا 255

```vb
Rnd(0,255)
```

* example color Random:

```vb
Dim r As Int = Rnd(0,255)
Dim g As Int = Rnd(0,255)
Dim b As Int = Rnd(0,255)
Panel.Color = Colors.RGB(r,g,b)

OR

Panel.Color = Colors.RGB(Rnd(0,255),Rnd(0,255),Rnd(0,255))
```

[hp](http://hemmatpoor.ir)
