# Java代码备份

## hello.java

```java
import java.util.Arrays;

public class hello {
    static int a5 = 3879;//静态变量

    public static void main(String[] args) {
        //简单输出
        System.out.println("------------------------------------------------------------------------------");
        System.out.println("Hello the world!");
        System.out.println();

        //初始化整型变量后再输出
        System.out.println("------------------------------------------------------------------------------");
        int a = 10;
        float b = 2.5f;
        double c = a / b;
        System.out.println("the value of c is " + c);
        System.out.println();

        //Unicode码的转换
        System.out.println("------------------------------------------------------------------------------");
        char d = '我', e = '你';
        int f = 1906;
        System.out.println("Unicode 我 is " + (int) d);
        System.out.println("Unicode 你 is " + (int) e);
        System.out.println("Unicode f  is " + (char) f);

        //转义字符
        System.out.println("------------------------------------------------------------------------------");
        System.out.println();
        char a1='\'' ,a2='\\' ,a3='\134' ,a4='\u6753';
        System.out.println(a1);
        System.out.println(a2);
        System.out.println(a3);//八进制
        System.out.println(a4);//十六进制

        //布尔型变量的使用
        System.out.println("------------------------------------------------------------------------------");
        boolean b3=true;
        boolean b1=true;
        boolean b2=false;
        System.out.println("Enter your answer");
        if(b3==b1)
            System.out.println("正确");
        else if(b3==b2)
            System.out.println("错误");
        System.out.println();

        //声明常量
        final double PI=3.1415926d;

        //逻辑运算符(必须定义为布尔型数据)
        boolean c1=b1 && b2;
        boolean c2=b1 || b2;

        //布尔型三元运算符
        boolean c3=43<83? true:false;

        //运算符优先级:
        /*
        1.增量和减量运算
        2.算术运算
        3.比较运算
        4.逻辑运算
        5.赋值运算
        */

        //隐式类型转换:低级到高级系统自动进行(byte<short<int<long<double)
        System.out.println("------------------------------------------------------------------------------");
        byte mybyte=127;
        float myfloat=150f;
        System.out.println("mybyte + myfloat = "+(mybyte+myfloat));

        //显式类型转换
        System.out.println("------------------------------------------------------------------------------");
        System.out.println();
        int c4=(int)45.94;
        long c5=(long)837.29f;
        int c6=(int)'g';
        System.out.println(c4);
        System.out.println(c5);
        System.out.println(c6);

        //复合语句:'{'开始, '}'结束
        //foreach语句
        System.out.println("------------------------------------------------------------------------------");
        System.out.println();
        int arr[]=new int[]{78,9,89};//数组的声明
        System.out.println("一维数组的元素:");
        for(int x:arr){
            System.out.println(x);
        }

        //菱形
        System.out.println("------------------------------------------------------------------------------");
        int lineCount = 17;// 输出的菱形有多少行，请赋值成奇数

        int maxLineNum = (lineCount + 1) / 2;// 菱形最多一行
        for (int i = 1; i <= maxLineNum; i++) {// 循环菱形数量越来越多的几行
            for (int space = 1; space <= maxLineNum - i; space++) {// 输出空格，数量=最后一行-当前行数
                System.out.print("  ");
            }
            for (int star = 1; star <= (i * 2) - 1; star++) {// 输出星号，数量=行数*2-1
                System.out.print("* ");
            }
            System.out.println();// 换行
        }
        //菱形下半部分
        int declineCount = lineCount - maxLineNum;// 计算剩下的几行，这几行星号的数量是递减的
        for (int i = 1; i <= declineCount; i++) {// 循环菱形数量越来越少的行数
            for (int space = 1; space <= i; space++) {// 输出空格，数量等于当前的行数
                System.out.print("  ");
            }
            for (int star = 1; star <= (declineCount - i + 1) * 2 - 1; star++) {// 输出星号，数量等于（总数-当前行数）*2-1
                System.out.print("* ");
            }
            System.out.println();
        }
        //创建一维数组
        // 先声明,再用new关键字进行内存分配
        int arr1[];
        arr1=new int[5];
        //声明和内存分配同时进行
        int arr2[] = new int[5];

        int arr3[]=new int[]{1,2,3,4,5,6,7,8,9,10};
        for(int i=0;i<10;i++){
            System.out.println(arr3[i]);
        }
        System.out.println();
        //二维数组
        int arr4[][]=new int[5][3];
        for(int i=0; i<arr4.length; i++){
            for(int j=0; j<arr4[i].length; j++){
                System.out.print(arr4[i][j]);
            }
            System.out.println();
        }
        //数组编程练习——数组的遍历
        System.out.println("------------------------------------------------------------------------------");
        char arr5[][]=new char[][]{{'春','眠','不','觉','晓'},
                {'处','处','闻','啼','鸟'},
                {'夜','来','风','雨','声'},
                {'花','落','知','多','少'}};
        //横板——for语句
        for(int i=0; i<arr5.length;i++){
            for(int j=0; j<arr5[i].length;j++){
                System.out.print(arr5[i][j]+" ");
            }
            System.out.println();
        }
        //横版——foreach语句
        System.out.println();
        int i=0;
        for(char x[]:arr5){
            i++;
            int j=0;
            for(char y:x){
                j++;
                if(i== arr5.length && i==x.length){
                    System.out.println(y);
                }else
                    System.out.print(y+" ");
            }
        }
        System.out.println();
        //竖版
        System.out.println();
        for(int j=0; j<5; j++) {
            for (i = 3; i >= 0; i--) {
                System.out.print(arr5[i][j] + " ");
            }
            System.out.println();
        }
        /*数  组  处  理*/
        System.out.println("------------------------------------------------------------------------------");
        //填充替换数组元素
        //将一值分配给数组每一个元素
        int arr6[]=new int[]{87,93,28,47};
        Arrays.fill(arr6,88);
        for(i=0; i<4; i++){
            System.out.println(arr6[i]);
        }
        //将指定的值分配给指定范围内的每个元素
        Arrays.fill(arr6,2,3, 99);
        for(i=0; i<4; i++)
            System.out.println(arr6[i]);
        System.out.println();
        //数组排序
        Arrays.sort(arr6);
        for(i=0;i<4;i++){
            System.out.println(arr6[i]);
        }
        //数组复制
        System.out.println();
        int arr7[]=Arrays.copyOf(arr6,3);
        for(i=0; i<3; i++)
            System.out.println(arr7[i]);
        System.out.println();
        int arr8[]=Arrays.copyOfRange(arr6,0,4);
        for(i=0;i<4;i++)
            System.out.println(arr8[i]);

        //查询数组-二分排序法
        //指定范围内
        Arrays.sort(arr8);
        int index = Arrays.binarySearch(arr8,0,4,99);
        System.out.println("99的位置"+index);
        //全部范围内
        System.out.println();
        Arrays.sort(arr7);
        index=Arrays.binarySearch(arr7,88);
        System.out.println("88的位置"+index);

        //数组排序算法
        System.out.println();
        System.out.println("------------------------------------------------------------------------------");
        //1.冒泡排序
        int maoArr[]=new int[]{68,80,70,87,88,67,86,38,78,96,29,89};
        for(i=1;i<maoArr.length;i++){
            for(int j=0;j<maoArr.length-i;j++){
                if(maoArr[j]>maoArr[j+1]){
                    int temp = maoArr[j];
                    maoArr[j] = maoArr[j+1];
                    maoArr[j+1] = temp;
                }
            }
        }
        for(i=0;i<12;i++){
            System.out.println("冒泡排序:"+maoArr[i]);
        }
        //2.直接选择排序
        System.out.println("------------------------------------------------------------------------------");
        int xuanArr[]=new int[]{16,54,96,84,15,95,13};
        for(i=1;i<xuanArr.length;i++){
            index=0;
            for(int j=1;j<=xuanArr.length-i;j++){
                if(xuanArr[j] > xuanArr[index]) {
                    index = j;
                }
            }
            int temp = xuanArr[xuanArr.length-i];
            xuanArr[xuanArr.length-i]=xuanArr[index];
            xuanArr[index] = temp;
        }
        for(i=0;i<xuanArr.length;i++){
            System.out.println("选择排序:"+xuanArr[i]);
        }
        //3.反转排序
        System.out.println("------------------------------------------------------------------------------");
        int fanArr[]=new int[]{1,2,3,4,5,6,7,8,9,10};
        for(i=0;i<fanArr.length/2;i++){
            int temp = fanArr[i];
            fanArr[i]=fanArr[fanArr.length-1-i];
            fanArr[fanArr.length-1-i] = temp;
        }
        for(i=0;i<fanArr.length;i++){
            System.out.println("反转排序:"+fanArr[i]);
        }
        //杨辉三角
        System.out.println("------------------------------------------------------------------------------");
        System.out.println("杨辉三角形:");
        int row=12;
        int yangArr[][]=new int[row+1][row+1];
        yangArr[0][0]=1;
        for(i=0;i<=row;i++){
            for(int j=1;j<=i;j++){
                if((i==0)||( i==j)){
                    yangArr[i][j]=1;
                    System.out.print(yangArr[i][j]+"  ");
                }
                else{
                    yangArr[i][j]=yangArr[i-1][j-1] + yangArr[i-1][j];
                    System.out.print(yangArr[i][j]+" ");
                }
            }
            System.out.println();
        }

        /*第二周学习*/
        //类与对象
        System.out.println("------------------------------------------------------------------------------");
    }
}
```
