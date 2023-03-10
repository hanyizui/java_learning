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

### 类
1.static关键字
- 静态变量/方法通过类.变量/方法来调用
- 静态导入包`import static ...`

2.final关键字

3.abstract
- 抽象类：内部可创建抽象方法，无法被实例化
- 抽象方法：只有方法名称，没有方法实现——必须由子类重写

4.代码块
- 分类
  - （匿名）代码块
  - 静态代码块：只执行一次
- 执行顺序: 静态代码块->代码块->构造方法

### 接口
1.特点
- 需要有实现类——必须重写接口中的方法
- 可以多继承
- 不能被实例化——没有构造方法

2.定义
- 方法：默认`public abstract`，可不写
- 常量：修饰`public static final`

### 内部类
1.定义方法
- `Outer.Inner inner = outer.new Inner();`

2.特点：
- 一个java类中可以有多个class类，但只能有一个public class；

