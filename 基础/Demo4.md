```java
package 基础;

import com.sun.scenario.effect.impl.sw.sse.SSEBlend_SRC_OUTPeer;

import java.sql.SQLOutput;

public class Demo4 {
    public static void main(String[] args) {
        //++ 自加 --自减  一元运算
        int a=3;//a=a+1

        int b=a++;//a++  a=a+1;执行代码后，先给b赋值,再自增

        int c=++a;//++a  a=a+1;执行代码前，先自增,再给c赋值
        System.out.println(a);
        System.out.println(b);
        System.out.println(c);
        //幂运算
        double pow =Math.pow(3,2);
        System.out.println(pow);
        int h=3;
        int n=h++;

        System.out.println(h);
        System.out.println(n);

    }
}
```