```java
System.out.println(object instanceof Student);//true
```

instanceof判断it是否为number子类

左边是对象，右边是类

**测试类**必须得是继承树的同一分支或存在继承关系，否则编译器会报错。

object>Person>student

```java
Person student =new Student();
//高      //指向         //低
//强制类型转换     父类转化为子类
（(Student obj)）.go
//可以使用低类的方法，高转低要使用强制转化  ，低转高不用强制
```

1.父类引用指向子类的对象

2.把子类转化为父类，向上转化

父类类名   父类对象名 = 子类实例

```java
Dog dog=new dog();//创建对象
Animal an = dog;//父类类名   父类对象名 = 子类实例
        Student student=new Student();
        student.say();
        Person person=student;
        person.getMoney();
        student.getMoney();//子类转为父类调用父类方法
```

3.把父类转化为子类，向下转化：强制转化

父类类名   父类对象名 = 子类实例；

子类类名  子类对象名=（子类名）父类对象名；

```java
Animal an=new Dog;//向上转化 子类→父类
Dog dog=(Dog)an;//向下转化
```

