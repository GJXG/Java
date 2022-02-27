```java
package 数组;

import java.lang.reflect.Array;
import java.util.Arrays;

public class Demo8 {
    public static void main(String[] args) {
        int [] d={1,6,66,76,88,999,355};
        int [] sort = sort (d);
        System.out.println(Arrays.toString(sort));

    }
    public static int[] sort(int[] array)  {
        //临时变量
        int temp =0;
        //外层循环  判断要走多少次
        for (int i=0;i<array.length-1;i++){
            //内层循环  比阶判断两个数，如果第一个数，比第二个大，则交换位置
            for (int j=0;j<array.length-1-i;j++){
                if (array[j+1]<array[j]){
                   temp= array[j];
                    array[j]=array[j+1];
                    array [j+1]=temp;
                }
            }

        }
        return array;
    }
}
```