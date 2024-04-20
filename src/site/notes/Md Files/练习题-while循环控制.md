---
{"dg-publish":true,"permalink":"/Md Files/练习题-while循环控制/","dgPassFrontmatter":true}
---

![练习题-while循环控制-1.png](/img/user/Pictures/%E7%BB%83%E4%B9%A0%E9%A2%98-while%E5%BE%AA%E7%8E%AF%E6%8E%A7%E5%88%B6-1.png)
```java
public class WhileExercise01{
	public static void main(String[] args){
		int i = 1;
		while(i <= 100){
			if(i % 3 == 0){
				System.out.println("i=" + i);
			}
			i++;
		}
	}
}
```
![练习题-while循环控制-2.png](/img/user/Pictures/%E7%BB%83%E4%B9%A0%E9%A2%98-while%E5%BE%AA%E7%8E%AF%E6%8E%A7%E5%88%B6-2.png)
```java
public class WhileExercise02{
	public static void main(String[] args){
		int i = 40;
		while(i <= 200){
			if(i % 2 == 0){
				System.out.println("i=" + i);
			}
			i++;
		}
	}
}
```