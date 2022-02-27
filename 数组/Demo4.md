```java
package 数组;

public class Demo4 {
    public static void main(String[] args) {
        int [] arrays ={1,2,3,4,5};
        //打印数组元素
        for (int i=0;i < arrays.length;i++){
            System.out.println(arrays[i]);
        }
        System.out.println("=====================");
        int sum =0;
        for (int j=0;j<arrays.length;j++){
            sum =sum +arrays[j];

        }
        System.out.println(sum);
        //寻找数组中最大元素
        int max=arrays[0];
        for (int i=0;i< arrays.length;i++){
            if (arrays[i]>max){
                max=arrays[i];
            }

        } System.out.println("max="+max);
    }
}
```