# 添加包含视图的控制器

![](http://img.hkwork3.top/blog/5/1.jpg)
![](http://img.hkwork3.top/blog/5/2.jpg)
![](http://img.hkwork3.top/blog/5/3.jpg)

# 执行以上添加“包含视图的MVC5控制器(使用Entity Framework)时报错

![](http://img.hkwork3.top/blog/5/4.jpg)

# 解决方案

## 在解决方案资源管理器中找到**packages.config**
![](http://img.hkwork3.top/blog/5/5.jpg)

## 注释掉**EntityFramework**和**EntityFramework.zh-Hans 6.2.0**
![](http://img.hkwork3.top/blog/5/6.jpg)

- **记得保存**

## 再次执行添加包含视图的控制器，已经可以使用了

- 生成的控制器
![](http://img.hkwork3.top/blog/5/7.jpg)

- 生成的视图
![](http://img.hkwork3.top/blog/5/8.jpg)



参考博客：CSDN:[我是一只小小鱼~](https://blog.csdn.net/qq_42335551/article/details/108181657)