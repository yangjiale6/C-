# C-#include <stdio.h>
#include<string.h>
#include<windows.h>
#include<stdlib.h>
int main()
{
	int i = 0;
	char password[20]={0};
	for (i = 0; i < 3; i++)
	{
		printf("请输入密码：>");
		scanf_s("%s", &password, sizeof(password));
		if (strcmp(password,"123abc")==0)
		{
			printf("登录成功\n");
			break;
		}
		else
		{
			printf("密码错误\n");
		}
	}if (i == 3)
		printf("三次密码均错误，退出程序\n");
	return 0;
}
