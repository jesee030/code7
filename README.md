# code7

新闻阅读器+登录页面

# 总结

1.在src/main/java/com/example/code7/NewsAdapter.java中 ImageView
ivImage的setImageResource要更换成setImageBitmap

原因是News中新添加bitmap属性传递image source

2.src/main/java/com/example/code7/MainActivity.java中setContentView布局为activity_main而非activity_login

3.src/main/res/layout/activity_main.xml中设置ListView控件属性如下即可实现新闻间隔:

``` xml
        android:divider="@android:color/transparent"
        android:dividerHeight="8dp"
```

4.Button 圆角设置:
src/main/res/drawable/shape.xml内设置属性android:radius 然后在Button，设置background属性即可 android:background="
@drawable/上面那个shape的文件名字"

# 参考

https://xxgqin.gitbook.io/android/ch04/ch04-2
