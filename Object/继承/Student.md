```java
package Object.Demo5;
//子类     子类继承了父类，就会拥有父类的全部方法
//在Java的所有的类中都默认直接或间接继承object
public class Student extends Person{
    public static void main(String[] args) {
    Student student=new Student();
    student.say();

        System.out.println(student.getMoney());
    }
//ctrl+h 可以查询这个类继承自那个类
}
```

