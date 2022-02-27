```java
package 方法;

public class Demo6 {
    //递归思想  尽量别用
    public static void main(String[] args) {
        System.out.println(f(10));
        //2!  2*1
        //3!  3*2*1  阶乘

    }
    //2 2 * f(1)
    //3 3 * f(2)
    public static int f(int n){
        //阶乘代码
        if (n==1){
            return 1;
        }else {
            return n*f(n-1);
        }
    }
}
```