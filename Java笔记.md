###Hello World
```
public class Main
{
  public static void main(String[] args)
  {
      System.out.println("Hello World");
  }
}
```
###数据类型
```
"hello world"    //字符串
213             //整数
12345678L      //长整数
浮点数类型: double高精度，float低精度
3.1415F      //float
true,false  //布尔
```
###运算符&关系运算符
```
"Pi="+3.1415    //字符串+数字
"Pi="+"3.1415" //字符串+字符串
10<20         //true
10==20       //false
```
###变量&变量类型
```
int i = 20;           //定义变量，整数型
double pi=3.1415;    //浮点型
String s="Hello";   //字符串
long v=123456486L; //长整型
boolean b=true;   //布尔型
```
###条件语句
if语句
```
int i=5;
if (i > 0)
{
System.out.println("i greater than 0");
}
```
if-else语句
```
int i=5;
if (i>6)
{
System.out.println("i >6");
}
else
{
System.out.println("i<=6");
}
```
while语句
```
int i=0;
while (i<=5)
{
System.out.println(i);
i++;
}
```
for循环语句
```
for (int i=0;i<=5;i++)
{
System.out.println(i);
}
```
###静态方法
```
public class Main
{
	public static void main(String[] args)
	{
		print("Hello");
		
	}
	
	static void print(String str)
	{
		System.out.println(str);
	}
}
```
有参数的静态方法
```
public static void main(String[] args)
{
int sum=mult(10,30);
System.out.println(sum);
}
static int mult(int a,int b)
{
return a+b;
}
```