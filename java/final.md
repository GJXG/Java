final表示**最终的，不可变的**。

final不可以被继承

```java
final class A{
    //A 是没有子孙的
}
class B extends A{
    //错误的, 无法从最终类A进行继承
    //B类继承A类 相当于对A类功能进行扩展
    //如果不希望别人对A类进行扩展，可以给A类加final关键字，如String类
}

```

用final写的方法无法被继承

final修饰的实例变量(必须手动赋值，只能赋值一次)

```java
/*
一般情况下
实例变量如果还没有赋值的话，系统会赋默认值

final 修饰实例变量：
系统不负责赋默认值，要求程序员必须手动赋值，只能赋一次，
这个手动赋值，在变量后面赋值可以，在构造方法中赋值也可以



*/
public class FinalTest02(){
    public static void main(String[]args){
        
    }
}


class User{
    //实例变量
    
    //错误： 变量age未在默认构造器中初始化
    //final int age;
    final int age=10;
    
    //在构造方法中赋值 weight只赋一次值
    final double weight;
    //构造方法
    public User(){   
        this.weight=80;
        //系统赋默认值在这个时候,final修饰后，系统不会赋值
        //this.weight=0;
     
    }
    
    
}

```

```java
public class Hero {
    String name;
    float hp;
    float armor;
    int movespeed;

    public static void main(String[] args) {
        final Hero hero;
        hero =new Hero();//引用final需要将Hero进行实例化
        hero.name="廉颇";//每个数据名只可以赋值一次，若再次赋值会造成上一次赋值失去作用
        hero.movespeed=650;
        hero.hp=8976;
        hero.armor=780;
    }
}

```

