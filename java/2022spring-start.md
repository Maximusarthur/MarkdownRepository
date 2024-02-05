## cainiao.java

```java
import java.util.Scanner;

public class cainiao {
    public static void main(String args[]) {
        System.out.println();
        System.out.println("wo shi yi ge bu zhuan zhu de ren !");
        char you = '\u4F60';
        char ChinaWord = '中';
        System.out.println("you:" + you);
        System.out.println("汉字ChinaWord:" + (int) ChinaWord);
        //输入基本数据
        System.out.println("-----------------------------------------------------------------------------");
        System.out.println("输入基本数据：");
        Scanner reader = new Scanner(System.in);
        double sum = 0;
        double x = reader.nextDouble();
        while (x != 0) {
            sum = sum + x;
            x = reader.nextDouble();
        }
        System.out.println("sum:" + sum);
        //输出一定范围内的随机数
        System.out.println((int)(Math.random()*100));//100代表100以内的随机数
  }
}
```
