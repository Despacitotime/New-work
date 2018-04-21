# New-work
for basic learning

1.
#include <stdio.h>

int main()
{
	printf("Hello World!\n");
	
	return 0;
}

2.
#include <stdio.h>

int main()
{
	printf("%d",12+23);
	
	return 0;
}

3.
#include <stdio.h>

int main()
{
	printf("12+34=%d",12+34);
	
	return 0;
}

4.
#include <stdio.h>

int main()
{
	int price=0;
	printf("请输入金额(元)：");
	scanf("%d",&price);
	
	int change=100-price;
	printf("找您%d元。\n",change);
}

5.
#include <stdio.h>

int main()
{
	int amount=100;
	int price=0;
	
	printf("请输入金额(元)：");
	scanf("%d\n",&price);
	
	printf("请输入票面(元)：");
	scanf("%d\n",&amount); 
	
	int change=amount-price;
	
	printf("找您%d元。\n",change);
	
	return 0;
}
修改版：
#include <stdio.h>

int main()
{
	int amount=100;
	int price=0;
	
	printf("请输入票面(元)：");
	scanf("%d",&amount); 
	
	printf("请输入金额(元)：");
	scanf("%d",&price);
	
	int change=amount-price;
	
	printf("找您%d元。\n",change);
	
	return 0;
}

6.
#include <stdio.h>

int main()
{
	int a;
	int b;
	
	printf("请输入两个整数:");
	scanf("%d %d",&a,&b);
	printf("%d+%d=%d\n",a,b,a+b);
	
	return 0;
}

7.
#include <stdio.h>

int main()
{
	printf("请分别输入身高的英尺和英寸，""如输入\"5 7\"表示5英尺7英寸:");
	
	int foot;
	int inch;
	
	scanf("%d %d",&foot,&inch);
	
	printf("身高是%f米。\n",((foot+inch/12)*0.3048));
	
	return 0;
}

#include <stdio.h>

int main()
{
	printf("请分别输入身高的英尺和英寸，""如输入\"5 7\"表示5英尺7英寸:");
	
	int foot;
	int inch;
	
	scanf("%d %d",&foot,&inch);
	
	printf("身高是%f米。\n",((foot+inch/12.0)*0.3048));
	
	return 0;
}
#include <stdio.h>

int main()
{
	printf("请分别输入身高的英尺和英寸，""如输入\"5 7\"表示5英尺7英寸:");
	
	double foot;
	double inch;
	
	scanf("%lf %lf",&foot,&inch);
	
	printf("身高是%f米。\n",((foot+inch/12)*0.3048));
	
	return 0;
}

8.
#include <stdio.h>

int main()
{
	int hour1,minute1;
	int hour2,minute2;
	
	scanf("%d %d",&hour1,&minute1);
	scanf("%d %d",&hour2,&minute2);
	
	int t1=hour1*60+minute1;
	int t2=hour2*60+minute2;
	int d=t2-t1;
	
	printf("%d %d",d/60,d%60);
	
	return 0;
}

9.
#include <stdio.h>

int main()
{
	int a,b;
	
	scanf("%d %d",&a,&b);
	
	double c=(a+b)/2;
	
	printf("%d与%d的平均值为%f\n",a,b,c);
	
	return 0;
}

10.
#include <stdio.h>

int main()
{
	int a=5;
	int b=6;
	int t;
	t=a;
	a=b;
	b=t;
	
	printf("a=%d b=%d",a,b);
	
	return 0;
}

11.#include <stdio.h>

int main()
{
	int a=5;
	
	printf("a++=%d\n",a++);
	printf("a=%d\n",a);
	
	printf("++a=%d\n",++a);
	printf("a=%d\n",a);
		
	return 0;
}

12.
#include <stdio.h>
int main()
{
  printf("************\n");
  printf("  Welcome   \n");
  printf("************\n");
  
  return 0;
}

13.
#include <stdio.h>
int main()
{
  int a;
  scanf("%d",&a);
  int b;
  b=a%10*100+a%100/10*10+a/100;
  printf("%d",b);
  
  return 0;
}

14.
int main()
{
	int hour1,minute1;
	int hour2,minute2;
	
	scanf("%d %d",&hour1,&minute1);
	scanf("%d %d",&hour2,&minute2);
	
	int hour=hour2-hour1;
	int minute=minute2-minute1;
	if(minute<0){
		minute=minute+60;
		hour --;
	}
	
	printf("时间差是%d小时%d分",hour,minute);
	
	return 0;
}

15.
#include <stdio.h>

int main()
{

	const int MINOR = 35;

	int age = 0;

	printf("请输入你的年龄: ");
	scanf("%d", &age);

	printf("你的年龄是%d岁。\n", age);

	if ( age < MINOR ) {
    	printf("年轻是美好的，");
	}

	printf("年龄决定了你的精神世界，好好珍惜吧。\n");

	return 0;
}

16.
#include <stdio.h>

int main()
{
	//	初始化
	int price = 0;
	int bill = 0;
	//	读入金额和票面
	printf("请输入金额：");
	scanf("%d", &price);
	printf("请输入票面：");
	scanf("%d", &bill);
	//	计算找零
	printf("应该找您：%d\n", bill - price);

	return 0;
}

#include <stdio.h>

int main()
{
	//	初始化
	int price = 0;
	int bill = 0;
	//	读入金额和票面
	printf("请输入金额：");
	scanf("%d", &price);
	printf("请输入票面：");
	scanf("%d", &bill);
	//	计算找零
	if ( bill >= price ) {
		printf("应该找您：%d\n", bill - price);
	}

	return 0;
}

#include <stdio.h>

int main()
{
	//	初始化
	int price = 0;
	int bill = 0;
	//	读入金额和票面
	printf("请输入金额：");
	scanf("%d", &price);
	printf("请输入票面：");
	scanf("%d", &bill);
	//	计算找零
	if ( bill >= price ) {
		printf("应该找您：%d\n", bill - price);
	} else {
		printf("你的钱不够\n");
	}

	return 0;
}
17.
#include <stdio.h>

int main()
{
	int a,b;

	printf("请输入两个整数：");
	scanf("%d %d", &a, &b);
	
	int max = b;
	if ( a > b ) {
		max = a;
	}

	printf("大的那个是%d\n", max);

	return 0;
}
//	max3.c
#include <stdio.h>

int main()
{
	int a,b,c;
	scanf("%d %d %d", &a, &b, &c);

	int max = 0;

	if ( a>b ) {
		if ( a>c ) {
			max = a;
		} else {
			max = c;
		}
	} else {
		if ( b>c ) {
			max = b;
		} else {
			max = c;
		}
	}

	printf("The max is %d\n", max);

	return 0;
}
18.
#include <stdio.h>

int main()
{
	const double RATE = 8.25;  
	const int STANDARD = 40;   
	double pay = 0.0;
	int hours;

	printf("请输入工作的小时数: ");
	scanf("%d", &hours);
	printf("\n");
	if (hours > STANDARD)
   		pay = STANDARD * RATE + 
   			(hours-STANDARD) * (RATE * 1.5);
	else
   		pay = hours * RATE;
	printf("应付工资: %f\n", pay);

	return 0;
}
19.
#include <stdio.h>

int main()
{
	const int PASS=60;
	int score;

	printf("请输入成绩: ");
	scanf("%d", &score);
	
	printf("你输入的成绩是%d.\n", score);
	if ( score < PASS )
		printf("很遗憾，这个成绩没有及格。");
	else {
		printf("祝贺你，这个成绩及格了。");
		printf("再见\n");
	}

	return 0;
}

20.#include <stdio.h>
int main()
{
	int a,b,c;
	scanf("%d %d %d",&a,&b,&c);
	
	int max=0;
	
	if(a>b){
		if(a>c){
			max=a;
		}else{
			max=c;
		}
	}else{
		if(b>c){
			max=b;
		}else{
			max=c;
		}
	}
	
	printf("The max is %d\n",max);
}

21.#include <stdio.h>
int main()
{
	const int READY=24;
	int code=0;
	int count=0;
	
	scanf("%d %d",&code,&count);
	if(code == READY){
		if(count<20)
		printf("一切正常\n");
	}else{
		printf("继续等待\n"); 
	}
	return 0;
}

22.
#include <stdio.h>

int main()
{
	int a,b;
	scanf("%d",&a);
	
	b=a%10*100+a%100/10*10+a/100;
	
	printf("%d",b);
	
	return 0;
}

23.#include <stdio.h>
int main()
{
int x;
int n=1;
scanf("%d",&x);

if(x>999){
	n=4;
}else if(x>99){
	n=3;
}else if(x>9){
	n=2;
}

printf("%d\n",n);
return 0;
}

24.#include <stdio.h>
int main()
{
int x;
int n=0;
scanf("%d",&x);
n++;
x/=10;
while(x>0){
	n++;
	x/=10;
}

printf("%d\n",n);
return 0;
}
由于计算机的数位限制，只能计算10位以下的数字
25.
