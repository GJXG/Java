```java
package how2j;

import java.util.Scanner;

public class BMI {
    public static void main(String[] args) {
        Scanner scanner=new Scanner(System.in);
        System.out.println("请输入身高(m):");
        float height=scanner.nextFloat();//定义身高的类型
        if (height<=3){
            System.out.println("身高为："+height);
        }else {
            System.out.println("输入错误");
        }
        System.out.println("请输入体重(kg)");
        float weight=scanner.nextFloat();//定义体重类型
        if (weight<=200){
            System.out.println("体重为："+weight);
        }else {
            System.out.println("输入错误");
        }
        scanner .close();
        float BMI=weight/(height*height);
        System.out.println("当前BMI："+BMI);

       if(BMI<18.5)
       {
           System.out.println("体重过轻");
       }else if (18.5<=BMI&&BMI< 24)
       {
           System.out.println("正常范围");
       }else if (24<=BMI&&BMI<27){
        System.out.println("体重过重");
       }else if (27<=BMI&&BMI<30){
           System.out.println("轻度肥胖");
       }else if (30<=BMI&&BMI<35){
           System.out.println("中度肥胖");
       }else if (35<=BMI){
           System.out.println("重度肥胖");
       }

    }

}
```