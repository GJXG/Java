```java

package Object.Demo1;

public class Demo1 {
    public static void main(String[] args) {
        //类：抽象的 ,实例化
        //类实例化后返回一个自己的对象
        //student对象就是一个Student类的具体实例
        Student xiaoming=new Student();
        Student xiaohong=new Student();
        xiaoming.name="小明";
        xiaoming.age=34;
        xiaohong.name="小红";
        xiaohong.age=20;
        System.out.println(xiaoming.name);
        System.out.println(xiaoming.age);
        System.out.println(xiaohong.name);
        System.out.println(xiaohong.age);
    }
}
```