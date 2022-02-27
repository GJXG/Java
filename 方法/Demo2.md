```java
package 方法;

public class Demo2 {
    public static void main(String[] args) {
      int max=max(8,8);
        System.out.println(max);
    }
//比大小
    private static int max(int h, int u) {
        int r =0;
        if (h==u){
            System.out.println("h==u");
            return 0;//终止方法
        }
        if (h>u){
            r=h;
        }else {
            r=u;
        }
        return r;//返回值
    }
}
```