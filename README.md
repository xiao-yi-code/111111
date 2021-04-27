创建一个结构体类型
struct Book
{
	char name[20];//c语言程序设计
	short price;//55
	int hao;
};//一定要有;来结束
int main()
{
	利用结构体类型 创建一个该类型的结构体变量
	struct Book b1 = {"C语言程序设计",55,8989};
	struct Book* pb = &b1;
	*/
	->  结构体指针->成员
	/*printf("书名：%s\n",pb->name);
	printf("价格：%d\n",pb->price);
	printf("编号：%d\n",pb->hao);
	*/

	.  结构体变量.成员
	printf("书名：%s\n",(*pb).name);
	printf("价格：%d\n",(*pb).price);
	printf("编号：%d\n",(*pb).hao);

	/*
	printf("书名：%s\n",b1.name);
	printf("价格：%d\n",b1.price);
	printf("编号：%d\n",b1.hao);
	b1.price = 45;
	printf("修改后的价格：%d\n",b1.price);
	*/
return 0;
}
