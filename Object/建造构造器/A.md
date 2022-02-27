```java
package Object.Demo2;

public class A {
   String name;
   int age;
//alt+insert 构造器中选择 Select为无参构造器
    public A() {
    }
    //alt+insert 构造器中选择 OK为有参构造器
    public A(String name) {
        this.name = name;
    }
//alt+insert 构造器中选择 OK为有参构造器  Ctrl可以全部生成有参构造器
    public A(String name, int age) {
        this.name = name;
        this.age = age;
    }


}
```