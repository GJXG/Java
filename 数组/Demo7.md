```java
package 数组;

import java.util.Arrays;

public class Demo7 {
    public static void main(String[] args) {


    int[]a ={1,2,3,7,998,888888};
    //System.out.println(a);


      Arrays.sort(a);//数组排序:升序
         System.out.println(Arrays.toString(a));//打印数组  Arrays.toString(a)
        Arrays.fill(a,0);//数组填充
        System.out.println(Arrays.toString(a));
    }
}
```