# Hospital-Security
//grand challenge project
#define _CRT_SECURE_NO_WARNINGS
#include<time.h>
#include<stdio.h>
#include<dos.h>
#include<conio.h>

int main(void) {
  char temp[100];/*creates a string array of characters, stores 100 characters
				   defines a limit of how many characters we can have so that it
				   does not take up more storage than necessary.*/

	time_t current_time = time(NULL);//setting the variable time to the current time
	struct tm *tm = localtime(&current_time);
	strftime(temp, sizeof(temp), "%c", tm);
	printf("\nCurrent Date and Time:\n");
	printf("\n%s\n\n", temp);

	getchar();
	return 0;
}
	
