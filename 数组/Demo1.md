```java
package 数组;

public class Demo1 {
    public static void main(String[] args) {//数组
        int[] nums;//定义   申明一个数组
        //int nums2[]; c++与c语言用法
        nums =new int[10];//可以存储10个int类型数字  创建一个数组
        //给数组赋值
        nums[0]=1;//从0开始索引
        nums[1]=2;
        nums[2]=3;
        nums[3]=4;
        nums[4]=5;
        nums[5]=6;
        nums[6]=7;
        nums[7]=8;
        nums[8]=9;
        nums[9]=10;
        System.out.println(nums[9]);
        //计算所有元素的和
        int sum =0;
        for (int i = 0; i <nums.length; i++){//nums.length 为数组长度
            sum =sum + nums [i];

        }System.out.println("总和为"+sum);
    }
}
```