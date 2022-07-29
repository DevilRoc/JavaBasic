## 数据类型

```java
public class VariableTest {
    public static void main(String[] args) {
        //基本数据类型
        int myAge = 18;
        double myWeight = 60.1;
        char myCup = 'A';
        boolean isMale = true;
        //引用数据类型
        String myName = "剪刀手罗克";
        int[] myEye = new int[]{1, 2};
    }
}
```

## 整型变量

```java
public class VariableTest {
    public static void main(String[] args) {
        byte b1 = 127;//一个字节
        short s1 = 32767;//两个字节
        int i1 = 21_4748_3647;//四个字节
        long l1 = 922_3372_0368_5477_5807L;//八个字节
    }
}
```

## 浮点类型

```java
public class VariableTest {
    public static void main(String[] args) {
      float f1 = 123.456f;//6~7个有效数字(要记得加字母f)
      double d1 = 12345.6789012345;//15~16个有效数字
      System.out.println(d1);
    }
}
```

## 字符类型

```java
public class VariableTest {
    public static void main(String[] args) {
        char c1 = 'a';
        char c2 = '\u7231';
        char c3 = '爱';
        char c4 = '\n';
        char c5 = '\t';
    }
}
```

## 布尔类型

```java
public class VariableTest {
    public static void main(String[] args) {
        boolean b1 = true;
        boolean b2 = 5 > 4;
        boolean b3 = 5 > 4 || 4 < 5;
    }
}
```

## 字符串类型

```java
public class VariableTest {
    public static void main(String[] args) {
        String s1 = "";
        int i1 = 7231;
        String s2 = s1 + i1;//字符串+别的类型变量会自动转换成字符串
    }
}
```
