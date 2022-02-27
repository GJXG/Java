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