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


