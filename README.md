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

