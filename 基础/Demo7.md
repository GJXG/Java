```java
package 基础;

public class Demo7 {
    public static void main(String[] args) {
        int a=10;
        int b=20;
        a+=b;//a=a+b
        a-=b;//a=a-b
        //字符串连接符    存在先后顺序""直接归为string类型  若""在前则两个数字连在一起
        //若""在后则两个数字加在一起
        System.out.println(""+a+b);
        System.out.println(a+b+"");
        System.out.println();
    }
}
```