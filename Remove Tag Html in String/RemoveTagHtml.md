# Remove Tag Html Convert String

اگر شما برای نمایش محتوا در برنامه از وب ویو استفاده میکنید , شاید گاهی مواقع بخواهید متن ساده ( بدون کد ها و تگ های HTML ) از وب ویو دریافت کنید ( مثلا برای اشتراک گذاری متن و ... ) برای اینکار کافیست کتابخانه JavaObject را فعال کنید و کد زیر را به اکتیویتی مورد نظرتان اضافه کنید ( در خارج از Sub ها ) :

* javaCode:

```java
#if java
public static String html2text(String html) {
 return android.text.Html.fromHtml(html).toString();
}
#end if
```

برای مثال محتوای HTML ما به شکل زیر است که آن را در یک متغیر متنی با نام st1 قرار داده ایم :

* use:

```b4a
Dim st1 As String = "<html><p>Hello World !</p></html>"
Dim j As JavaObject
j.InitializeContext
Label1.Text = j.RunMethod("html2text",Array As Object(st1))
```

با اجرای کد بالا فقط عبارت Hello World ! بدون تگ های HTML در لیبل نمایش داده میشود ...

* exit

```b4a
before: <html><p>Hello World !</p></html>

after:  Hello World !
```

[hp](http://hemmatpoor.ir)
