```java
package Object.Demo7;

public class Application {
    public static void main(String[] args) {
        //一个对象的实际类型是确定的
        //new Student();
        //new Person();
        //Student 能调用自身的类型以及继承父类的类型
        Student s1=new Student();
        //父类的引用指向子类
        //Person 可以指向子类但是不可以调用子类的方法
        Person s2=new Student();//子类重写父类的方法，执行子类的方法
        Object s3=new Student();
        //能执行哪些方法主要看左边的类型与右边关系不大
        ((Student) s2).eat();
        s1.run();
    }
}
```

