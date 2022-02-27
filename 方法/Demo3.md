```java
package 方法;

public class Demo3 {
    public static void main(String[] args) {
       Demo3 demo3= new Demo3();
       demo3.method(9,3,7788,2113,35,5,7);
    }
    public void method(int x,int...i){
        System.out.println(i[4]);
    }
}
```