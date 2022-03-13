```java
package Scanner;

import java.util.Scanner;

public class Demo1 {
    public static void main(String[] args) {
        Scanner scanner=   new Scanner(System.in);
        System.out.println("使用next方式接收");
        //判断用户有没有输入字符串
        if(scanner .hasNext()){
        //使用next接收
            String str =scanner.next();//定义String类输入字符串
            System.out.println("输入的内容为："+str);
        }

        scanner.close();();//运行完后一定要输入该代码否则将继续运行
        

     }


}
```

## next（）：

1.一定要读到有效字符后才结束

2.    若有效字符前有间隔号，next（）方法会自动将空格号后的字符去掉
3. next（）方法不能带有空格的字符串

```
package Scanner;

import java.util.Scanner;

public class Demo2 {
    public static void main(String[] args) {
        Scanner scanner=new Scanner(System.in);
        System.out.println("使用nextLine方式接收");
        if(scanner .hasNextLine()){
            String str =scanner.nextLine();
            System.out.println("输入的内容为："+str);

        }
        scanner. close();//运行完后一定要输入该代码否则将继续运行
    }
}
```

## NextLine()：

1.以Enter为结束符

2.可以有空白间隔号

