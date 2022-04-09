# c-code
//函数递归
//练习一：接受一个整型值（无符号），按照顺序打印它的每一位。例如输入1234，输出1 2 3 4


void print(int n)
{
	if(n>9)
	{
		print(n / 10);
	}
	printf("%d ", n % 10);
}

int main()
{
	unsigned int num = 0;
	scanf_s ("%d", &num);
	print(num);
	return 0;
}
