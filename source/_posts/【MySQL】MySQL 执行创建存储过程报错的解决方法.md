# 源码
## 创建使用while循环插入数据的存储过程
```sql
设置mysql分隔符为//
delimiter // 
drop procedure if exists while1 ;
create procedure while1()
begin
declare i int default 0;
set i = 0 ;
while i < 10 do
insert into test_table(tname) values('TestName1');
set i = i + 1 ;
end while;
select * from test_table;
end 
// 
call while1();
delimiter ;
```
## 执行
执行后可以看到数据库中已经有了while1存储过程，证明命令已经成功执行

![](http://img.hkwork3.top/blog/1/0.png)

但是报错：`Error Code: 2014 Commands out of sync; you can't run this command now`

---

# 解决方法

**将上述语句中的**

```sql
drop procedure if exists while1 ;
```

**改为**

```sql
drop procedure id exists while1 //
```

# 问题解决