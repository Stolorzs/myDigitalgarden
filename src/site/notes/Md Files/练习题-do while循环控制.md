---
{"dg-publish":true,"permalink":"/md-files/do-while/","dgPassFrontmatter":true}
---

![练习题-do while循环控制-1.png](/img/user/Pictures/%E7%BB%83%E4%B9%A0%E9%A2%98-do%20while%E5%BE%AA%E7%8E%AF%E6%8E%A7%E5%88%B6-1.png)
```java
public class DoWhileExercise01{
	public static void main(String[] args){
		int i = 1;
		do{
			System.out.println(i);
			i++;
		}while(i <= 100);
	}
}
```
![练习题-do while循环控制-2.png](/img/user/Pictures/%E7%BB%83%E4%B9%A0%E9%A2%98-do%20while%E5%BE%AA%E7%8E%AF%E6%8E%A7%E5%88%B6-2.png)
```java
public class DoWhileExercise02{
	public static void main(String[] args){
		int i = 1;
		int sum = 0;
		do{
			sum += i;
			i++;
		}while(i <= 100);
		System.out.println("1-100的和为" + sum);
	}
}
```
![练习题-do while循环控制-3.png](/img/user/Pictures/%E7%BB%83%E4%B9%A0%E9%A2%98-do%20while%E5%BE%AA%E7%8E%AF%E6%8E%A7%E5%88%B6-3.png)
```java
public class DoWhileExercise03{
	public static void main(String[] args){
		int i = 1;
		int count = 0;
		do{
			if(i % 5 == 0 && i % 3 != 0){
				count++;
			}
			i++;
		}while(i <= 200);
		System.out.println("个数为" + count);
	}
}
```
![练习题-do while循环控制-4.png](/img/user/Pictures/%E7%BB%83%E4%B9%A0%E9%A2%98-do%20while%E5%BE%AA%E7%8E%AF%E6%8E%A7%E5%88%B6-4.png)
```java
import java.util.Scanner;
public class DoWhileExercise04{
	public static void main(String[] args){
		char answer = ' '; 
		Scanner myScanner = new Scanner(System.in);
		do{
			System.out.println("老韩使出了闪电五连鞭~");
			System.out.println("老韩问：还钱吗？y/n");
			answer = myScanner.next().charAt(0);
		}while(answer != 'y');
		System.out.println("饶了你 ");
	}
}
```