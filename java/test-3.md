习题三
一、问答题
1．关系运算符的运算结果是怎样的数据类型？
答：布尔型数据。
2．if语句中的条件表达式的值是否可以是int型？
答：可以。
3．while语句中的条件表达式的值是什么类型？
答：
4．switch语句中必须有default选项码？
答：不一定，可以省略。
5．在while语句的循环体中，执行break语句的效果是什么？
答：跳出循环体。
6．可以用for语句代替while语句的作用吗？
答：可以。
二、选择题
1．下列哪个叙述是正确的？（A）
A.  5.0/2+10的结果是double型数据。
B．(int)5.8+1.0的结果是int型数据。
C．'苹'+ '果'的结果是char型数据。
D．(short)10+'a'的结果是short型数据。
2．用下列哪个代码替换程序标注的【代码】会导致编译错误？
A．m-->0  B．m++>0  C．m = 0  D．m>100&&true
public class E {  
    public static void main (String args[ ]) {
      int m=10,n=0;
      while(【代码】) {
         n++;
      }  
    }
}
3．假设有int x=1;以下哪个代码导致“可能损失精度，找到int需要char”这样的编译错误。
A．short t=12+'a';  B．char c ='a'+1;  C．char m ='a'+x;  D．byte n ='a'+1;
三、阅读程序
1．下列程序的输出结果是什么？
public class E {  
public static void main (String args[ ])   {  
 char x='你',y='e',z='吃';
       if(x>'A'){
           y='苹';
           z='果';
        }
       else
          y='酸';
       z='甜';
       System.out.println(x+","+y+","+z);
   }
}
2.下列程序的输出结果是什么？
public class E {
  public static void main (String args[ ]) {
        char c = '\0';
        for(int i=1;i<=4;i++) {
          switch(i) {
             case 1:  c = 'J';
                     System.out.print(c);  
             case 2:  c = 'e';
                     System.out.print(c);
                     break;
             case 3:  c = 'p';
                     System.out.print(c);
             default: System.out.print("好");
          }   
        }
    }
}
3.下列程序的输出结果是什么？
public class E {
   public static void main (String []args)   {
      int x = 1,y = 6;
      while (y-->0) {
          x--;
      }
      System.out.print("x="+x+",y="+y);
   }
}
四、编程序题
1．编写应用程序求1!+2!+…+10!。
2．编写一个应用程序求100以内的全部素数。
3．分别用do-while和for循环计算1+1/2!+1/3!+1/4!…  … 的前20项和。
4．一个数如果恰好等于它的因子之和，这个数就称为“完数”。编写应用程序求1000之内的所有完数。
5．编写应用程序，使用for循环语句计算8+88+888…前10项之和。
6．编写应用程序，输出满足1+2+3…+n<8888的最大正整数n。
