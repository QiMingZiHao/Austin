//# Austin
//My own clutter
#include<stdio.h>
 //交换地址变量 
void sort(int *a)//排序 
{
	int i, j;
	for (i = 0; i < 10; i++)
		for(j=0;j<10-i-1;j++)
			if (*(a + j) > *(a + j + 1))
			{
				int temp = *(a + j);
				*(a + j) = *(a + j + 1);
				*(a + j + 1) = temp ;
			}
}
 
int main()
{
	//={34,2,56,54,13,67,89,57,8,16};
	int arr[10], i;
	void sort(int* a);//声明 
	for (i = 0; i < 10; i++)
	{	scanf("%d", &arr[i]);}
	
	sort(arr);
	for (i = 0; i < 10; i++)
	{	printf("%d  ", arr[i]);}
	
	return 0;
}
