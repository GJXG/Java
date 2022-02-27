```java
package Object.Demo2;

public class Person {
    //一个类即使什么都不写，就会存在一个方法
    //显示的定义构造器
    String name;
    int age;
    //实例化初始值  无参构造
    //1.使用new关键词，本质在调用构造器
    /*public Person(){

    }
    //有参构造：一旦定义有参构造，无参必须必须显示定义
    public Person(String name){
        this.name=name;
    }*/
    //alt+insert 生成构造器

    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }
}

```

