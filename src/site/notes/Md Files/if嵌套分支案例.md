---
{"dg-publish":true,"permalink":"/md-files/if/","dgPassFrontmatter":true}
---

![if嵌套分支案例-1.png](/img/user/Pictures/if%E5%B5%8C%E5%A5%97%E5%88%86%E6%94%AF%E6%A1%88%E4%BE%8B-1.png)
```java
import java.util.Scanner;
public class NestedIf{
	public static void main(String[] args){
		Scanner myScanner = new Scanner(System.in);
		System.out.println("请输入成绩");
		double score = myScanner.nextDouble();
		System.out.println("请输入性别(男or女)");
		char gender = myScanner.next().charAt(0);
		if(score >= 0 && ((gender == '男') || (gender == '女'))){
			if(score > 8.0){
				if(gender == '男'){
					System.out.println("您已进入男子组决赛");
				}else{
					System.out.println("您已进入女子组决赛");
				}
			}else{
					System.out.println("您被淘汰了");
			}
		}else{
			System.out.println("成绩或性别输入有误，请重新输入");
		}
	}
}
```

```java 
//错误
import java.util.Scanner;
public class NestedIf{
	public static void main(String[] args){
		Scanner myScanner = new Scanner(System.in);
		System.out.println("请输入成绩");
		double score = myScanner.nextDouble();
		System.out.println("请输入性别(男or女)");
		String gender = myScanner.next();
		if(score >= 0 && (gender == "男") || (gender == "女")){
			if(score > 8.0){
				if(gender == "男"){
					System.out.println("您已进入男子组决赛");
				}else{
					System.out.println("您已进入女子组决赛");
				}
			}else{
					System.out.println("您没有进入决赛");
			}
		}else{
			System.out.println("成绩或性别输入有误，请重新输入");
		}
	}
}
```