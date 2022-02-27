```java
package 基础;
//逻辑运算符
public class Demo5 {


    public static void main(String[] args) {
        // 与（and） 或（or） 非（取反）
        boolean a = true;
        boolean b =false;


        System.out.println("a&&b:"+(a&&b));//逻辑与运算：两个变量为真，结果才为true
        System.out.println("a||b:"+(a||b));//逻辑或运算：两个变量有一个为真，结果才为true
        System.out.println("!(a&&b):"+!(a&&b));//如果为真，则为假。如果为假,则结果为真

    }
}
```

