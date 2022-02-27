```java
package 数组;

public class Demo9 {
    public static void main(String[] args) {


        //创建一个二维数组  0：没有棋子 1：黑棋  2：白棋
        int[][] array1 = new int[11][11];//表示11行11列
        array1 [1][2]=1;//从第0行第0列开始
        array1 [2][3]=1;

        System.out.println("输出原始数组");
        for (int[] ints : array1) {
            for (int anInt : ints) {
                System.out.print(anInt+"\t");
            }
            System.out.println();
        }
        //转化为稀疏数组
        //获取有效值个数
        int sum =0;
        for (int i = 0; i <11 ; i++) {
            for (int j=0; j<11;j++){
                if (array1[i][j]!=0){
                    sum++;
                }
            }
        }
        System.out.println("有效值的个数"+sum);
        //创建一个稀疏数组的数组
        int [] [] array2 =new int[sum+1][3];
        array2 [0][0]=11;
        array2 [0][1]=11;
        array2 [0][2]=sum;
        int count=0;
        for (int i = 0; i <array1.length ; i++) {
            for (int j = 0; j < array1.length; j++) {
                if (array1[i][j]!=0){
                    count++;
                    array2[count][0]=i;
                    array2[count][1]=j;
                    array2[count][2]=array1[i][j];
                }

            }
        }
        System.out.println("输出稀疏数组");
        for (int i = 0; i <array2.length ; i++) {
            System.out.println(array2[i][0]+"\t"
                            +array2[i][1]+"\t"+
                            +array2[i][2]+"\t"
            );

        }
    }
}
```