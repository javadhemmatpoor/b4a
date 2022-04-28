# Detect Label Link

با استفاده از کد های زیر میتوانید لینک های موجود در متن یک Label را تشخیص دهید ( در واقع با استفاده از این کد رنگ لینک ها در لیبل تغییر میکند و با کلیک روی آنها لینک در مرورگر وب نمایش داده میشود )

ابتدا کتابخانه JavaObject را فعال کنید و کد زیر را به اکتیویتی مورد نظرتان اضافه کنید :

* java:

```java
#if java
import android.widget.TextView;
import android.text.util.Linkify;
public void link(TextView LaeblName){
 Linkify.addLinks(LaeblName, Linkify.ALL);
}
#end if
```

و در کد زیر لیبل مورد نظرتان را انتخاب کنید :

* use:

```vb
Dim j As JavaObject
j.InitializeContext
j.RunMethod("link",Array(label1))
```

[hp](http://hemmatpoor.ir)
