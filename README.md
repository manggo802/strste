문자 채움 함수 만들기
#include <stdio.h>

char* StrChr(char* pstring, char ch);

int main(void)
{
	char string[100];
	char* pos;

	strcpy(string, "this is a book");
	strset(string, '*');
	puts(string);

	strcpy(string, "this is a book");
	strset(string, '*');
	puts(string);

	return 0;
}

char* StrChr(char * pstring, char ch)
{
	char* start = pstring;

	while (*pstring)
	{
		*pstring++ = ch;
	}
	return start;
}
