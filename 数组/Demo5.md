```java
package 数组;

public class Demo5 {
    public static void main(String[] args) {
        int [] arrays ={1,2,3,4,5};
        //int array 数组中的每一个元素
        /*for (int array : arrays) {
            System.out.println(array);
        }
        printArray(arrays);*/
        int[] reverse =reverse(arrays);
        printArray(reverse);
    }
    //打印数组元素方法
    public static void printArray(int []arrays){
        for (int i= 0;i<arrays.length;i++){
            System.out.print(arrays[i]+" ");
        }
    }
    //反转数组方法
    public static int [] reverse(int[]  arrays){
        int  [] reault =new int[arrays.length];
        //反转
        for (int i = 0,j=reault.length-1 ; i <arrays.length ; i++,j--) {
           // reault[]=arrays[i]
            reault [j]=arrays[i];
        }
        return reault;
    }
}
```