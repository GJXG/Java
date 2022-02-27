```java
package 数组;

public class Demo6 {
    public static void main(String[] args) {
        //[4][2]  二维数组
        /*
        1,2  array[0]
        2,3  array[1]
        3,4  array[2]
        4,5  array[3]
         */
       /* int [] [] array  ={{1,2},{2,3},{3,4},{4,5}};
        printArray(array[0]);*/
        int [] [] array  ={{1,2},{2,3},{3,4},{4,5}};
        System.out.println(array[0][0]);//输出1  解析：在array第0组第0个元素

    }
    //打印数组
    public static void printArray(int []arrays){
        for (int i= 0;i<arrays.length;i++){
            System.out.print(arrays[i]+" ");
        }
    }
}
```