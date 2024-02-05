习题二
一、问答题
1．	什么叫标识符？标识符的规则是什么？false是否可以作为标识符。
2．	什么叫关键字？true和false是否是关键字？请说出6个关键字。
3．	Java的基本数据类型都是什么？
4．	float型常量和double型常量在表示上有什么区别？
5. 怎样获取一维数组的长度,怎样获取二维数组中一维数组的个数。
二、选择题
1．下列哪项字符序列可以做为标识符？
A. true
B. default
C. _int
D. good-class
2．下列哪三项是正确的float变量的声明？
 A. float foo = -1;
 B. float foo = 1.0;
 C. float foo = 42e1;
 D. float foo = 2.02f;
 E. float foo = 3.03d;
 F. float foo = 0x0123;
3．下列哪一项叙述是正确的？
A. char型字符在Unicode表中的位置范围是0至32767
B. char型字符在Unicode表中的位置范围是0至65535
C. char型字符在Unicode表中的位置范围是0至65536
D. char型字符在Unicode表中的位置范围是-32768至32767
4．以下哪两项是正确的char型变量的声明？
A. char ch = "R";
B. char ch = '\\'
C. char ch = 'ABCD';
D. char ch = "ABCD";
E. char ch = '\ucafe';
F. char ch = '\u10100'
5．下列程序中哪些【代码】是错误的？
public class E {
   public static void main(String args[]) {
      int x = 8;
      byte b = 127;     //【代码1】
      b = x;           //【代码2】
      x = 12L;         //【代码3】
      long y=8.0;       //【代码4】
      float z=6.89 ;     //【代码5】
   }
}
6．对于int a[] = new int[3];下列哪个叙述是错误的？
A. a.length的值是3。
B. a[1]的值是1。
C. a[0]的值是0。
D. a[a.length-1]的值等于a[2]的值。
三、阅读或调试程序
1．上机运行下列程序，注意观察输出的结果。
public class E {
 public static void main (String args[ ]) {
      for(int i=20302;i<=20322;i++) {
          System.out.println((char)i);
      }
    }
}
2．上机调试下列程序，注意System.out.print()和System.out.println()的区别。
public class OutputData {
  public static void main(String args[]) {
        int x=234,y=432;
        System.out.println(x+"<"+(2*x));
        System.out.print("我输出结果后不回车");
        System.out.println("我输出结果后自动回车到下一行");
        System.out.println("x+y= "+(x+y));
     }
}
3．上机调试下列程序，了解基本数据类型数据的取值范围。
public class E {
  public static void main(String args[]) {
     System.out.println("byte取值范围:"+Byte.MIN_VALUE+"至"+Byte.MAX_VALUE);
     System.out.println("short取值范围:"+Short.MIN_VALUE+"至"+Short.MAX_VALUE);
     System.out.println("int取值范围:"+Integer.MIN_VALUE+"至"+Integer.MAX_VALUE);
     System.out.println("long取值范围:"+Long.MIN_VALUE+"至"+Long.MAX_VALUE);
     System.out.println("float取值范围:"+Float.MIN_VALUE+"至"+Float.MAX_VALUE);
     System.out.println("double取值范围:"+Double.MIN_VALUE+"至"+Double.MAX_VALUE);
  }
}
4.下列程序标注的【代码1】，【代码2】的输出结果是什么？
public class E {
public static void main (String args[ ]){
long[] a = {1,2,3,4};
       long[] b = {100,200,300,400,500};
       b = a;
       System.out.println("数组b的长度:"+b.length); //【代码1】
       System.out.println("b[0]="+b[0]); //【代码2】
   }
}
5.下列程序标注的【代码1】，【代码2】的输出结果是什么？
public class E {
   public static void main(String args[]) {
     int [] a={10,20,30,40},b[]={{1,2},{4,5,6,7}};
     b[0] = a;
     b[0][1] = b[1][3];
     System.out.println(b[0][3]); //【代码1】
     System.out.println(a[1]);   //【代码2】
   }
}
四、编写程序
1．编写一个应用程序，给出汉字‘你’、‘我’、‘他’在Unicode表中的位置。
2．编写一个Java应用程序，输出全部的希腊字母。
