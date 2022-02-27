```java
package 方法;

public class Demo1 {
    public static void main(String[] args) {
        int sum =add(1,5,5);//可以有多个参数  加法
        System.out.println(sum);
        System.out.println("---------------------------------------------------------------------");
        int dot =g(8,2);//减法
        System.out.println(dot);
        System.out.println("---------------------------------------------------------------------");
        int cat =fly(100,10);//除法
        System.out.println(cat);
        System.out.println("---------------------------------------------------------------------");
        int dao =mo(7,9);//乘法
        System.out.println(dao);
        System.out.println("----------------------------------------------------------------------");
        odd();//直接引用下方odd的方法
        System.out.println("-----------------------------------------------------------");
        kpl();//直接引用下方kpl的方法
        System.out.println("-----------------------------------------------------------");
    }

    //加法  代码
    public static int add(int a, int b,int c){return a+b+c;}
    //减法  代码
    public static int g(int e,int f){
        return e-f;
    }
    //乘法  代码
    public static int mo(int j,int p){
        return j*p;
    }
    //除法  代码
    public static int fly(int r, int h){
        return r/h;
    }


    //能被五整除 代码
    public static void odd(){
        for (int l=0;l<100;l++){
            if (l % 5 == 0) {
                System.out.println(l+"\t");

            }
            }
        }
        public static void kpl(){
        for (int m=0;m<=1000;m++){
            if (m%7==0){
                System.out.println(m+"\t");
            }
        }
        }
}
```