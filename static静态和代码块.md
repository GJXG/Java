```java
private static int age;//静态变量
private double score;//非静态变量
Student s1=new Student();//将Student实例化，让Student不能够使用非静态变量,创建s1这个对象，使s1调用非静态变量
System.out.println(Student.age);
//System.out.println(Student.score);不能够调用非静态变量
System.out.println(s1.age);
System.out.println(s1.score);
new Student().run();//非静态方法调用方式
Student.go();//静态方法调用方式
```

完整代码

```java
package Object.Demo8;

public class Student {
    private static int age;//静态变量
    private double score;//非静态变量
public void run(){//非静态方法,不可以直接调用

}
public static void go(){//静态方法

}

    public static void main(String[] args) {
        Student s1=new Student();//将Student实例化，让Student不能够使用非静态变量,创建s1这个对象，使s1调用非静态变量
        System.out.println(Student.age);
        //System.out.println(Student.score);不能够调用非静态变量
        System.out.println(s1.age);
        System.out.println(s1.score);
       new Student().run();//非静态方法调用方式
        Student.go();//静态方法调用方式
    }
}

```

```java
package Object.Demo8;

public class Person {
    {
        //代码块（匿名代码块）
    }
    static {
        //静态代码块只执行一次
    }
}
```

执行顺序

静态代码块>代码块>构造器

```java
package Object.Demo8;
import static java.lang.Math.random;//静态导入包
import static java.lang.Math.PI;//静态导入包
public class test {
    public static void main(String[] args) {
        System.out.println(Math.random());
        System.out.println(PI);
    }
}

```

在上方输入静态导入包后可以在下方直接使用方法