# C-programming
Choose the middle number form the user input

#include <stdio.h>
#include <stdlib.h>

#pragma warning(disable:4996)


void main()
{
	int input1, input2, input3;
	int mid;

	printf("Enter 1st number >");
	scanf("%d", &input1);
	printf("Enter 2nd number >");
	scanf("%d", &input2);
	printf("Enter 3th number >");
	scanf("%d", &input3);


	if (input1 >= input2 && input1 <= input3 || input1 >= input3 && input1 <= input2)
	{
		mid = input1;

	}
	else
	{
		if (input2 >= input1 && input2 <= input3 || input2 >= input3 && input2 <= input1)
		{
			mid = input2;
		}
		else
		{
			mid = input3;
		}
		
	}

	printf("%d\n", mid);

	system("pause");
}
