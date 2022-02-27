```java
package 方法;

import java.util.Scanner;

public class Demo5 {
    public static void main(String[] args) {
        Scanner scanner=new Scanner(System.in);
        System.out.println("输入两个数字:");

        int a = scanner.nextInt();
        int b = scanner.nextInt();
        int sum= add (a,b);
        int dot=sub (a,b);
        int dao=mul(a,b);
        int cat=div(a,b);
        System.out.println("------------------------------------------------------------------------");
        System.out.println("两个数之和"+sum);
        System.out.println("两个数的差"+dot);
        System.out.println("两个数相乘"+dao);
        System.out.println("两个数相除"+cat);
    }
    public static int add(int a, int b)
    {return a+b;}
    public static int sub(int a,int b)
    {return a-b;}
    public static int mul(int a,int b)
    {return a*b;}
    public static int div(int a, int b)
    {int c=a/b;
        return c;}
}
```