```java
package Object.Demo5;
//父类
public class Person {
    //public int money=10_0000_0000;属性私有后不可以直接继承
    private int money =10_0000_0000;
    public void say(){
        System.out.println("说了一句话");
    }
    public int getMoney(){
        return money;
    }
}
```