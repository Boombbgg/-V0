#include <stdio.h>
#include <string.h>
void main()
{
	char a[] = "3+4";
	int b = a[0] - '0';
	int c = 0;
	for (int i = 1; i < strlen(a); i++)
	{
		if (a[i] == '+')
		{
			c = a[i + 1] - '0' + b;
			i++;
		}
		if (a[i] == '-')
		{
			c = a[i + 1] - '0' + b;
			i++;
		}
	}
	printf("%d\n", c);
  }
