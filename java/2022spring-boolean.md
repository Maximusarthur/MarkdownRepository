#2022spring-Boolean
```java
public class Boolean {
    public static void main(String args[]){
        boolean flag = true;
        flag &= true;
        System.out.println("true\t&=\ttrue\t==>\t"+ flag);
        flag = true;
        flag &= false;
        System.out.println("true\t&=\tfalse\t==>\t" + flag);
        flag = false;
        flag &= true;
        System.out.println("false\t&=\ttrue\t==>\t" + flag);
        flag = false;
        flag &= false;
        System.out.println("false\t&=\tfalse\t==>\t"+ flag+"\n");
        flag = true;
        flag |= true;
        System.out.println("true\t|=\ttrue\t==>\t" + flag);
        flag = true;
        flag |= false;
        System.out.println("true\t|=\tfalse\t==>\t" + flag);
        flag = false;
        flag |= true;
        System.out.println("false\t|=\ttrue\t==>\t" + flag);
        flag = false;
        flag |= false;
        System.out.println("false\t|=\tfalse\t==>\t" + flag+"\n");

        System.out.println("^=  相同为假，不同为真");
        flag = true;
        flag ^= true;
        System.out.println("true\t^=\ttrue\t==>\t" + flag);
        flag = true;
        flag ^= false;
        System.out.println("true\t^=\tfalse\t==>\t" + flag);
        flag = false;
        flag ^= true;
        System.out.println("false\t^=\ttrue\t==>\t" + flag);
        flag = false;
        flag ^= false;
        System.out.println("false\t^=\tfalse\t==>\t" + flag);
        boolean b;
        //布尔型的注意事项
        b = false;
        System.out.println("b is " + b);
        b = true;
        System.out.println("b is " + b);
        // a boolean value can control the if statement
        if(b) System.out.println("This is executed.");
        b = false;
        if(b) System.out.println("This is not executed.");
        // outcome of a relational operator is a boolean value
        System.out.println("10 > 9 is " + (10 > 9));
    }
}
```
