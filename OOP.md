### 多态
1.存在条件
- 有继承关系
- 子类重写父类方法
- 父类引用指向子类对象

2.重写
- 父类方法为static/final/private时无法重写

3.父子
- 父类引用指向子类对象，无法调用子类独有的方法，需要强制转换`(Father(son)).fun();`
- 子类可自动转换为父类`Father father=new Son();`

3.instanceof
```java
System.out.println(X instanceof Y);

```
