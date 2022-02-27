```java
package 方法;

public class Demo7 {
    public static void main(String[] args) {
        java.util.Scanner scanner= new java.util.Scanner(System.in);
        System.out.println("欢迎使用本计算器");

        System.out.println("\n");
        System.out.print("请输入需要计算的第一个数字");
        int num1 =scanner.nextInt();
        System.out.print("请输入运算符");
        String i=scanner.next();

        System.out.print("请输入需要计算的第二个数字");
        int num2=scanner.nextInt();
        switch (i){
            case "+":
                int result= num1+num2;
                System.out.println("运算结果为："+num1+" "+"+"+" "+num2+""+"="+result);
                break;
            case "-":
                 result=num1-num2;
                System.out.println("运算结果为："+num1+" "+"-"+""+num2+" "+"="+""+result);
                 break;
            case "*":
                result =num1*num2;
                System.out.println("运算结果为："+num1+" "+"*"+" "+num2+""+"="+result);
                break;
            case "/":
                result=num1/num2;
                System.out.println("运算结果为："+num1+" "+"/"+" "+num2+" "+"="+result);
                break;
            default:
                System.out.println("本系统不支持此运算");
        }
    }
}
```

