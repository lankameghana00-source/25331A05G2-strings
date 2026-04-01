#include <stdio.h>
#include <string.h>   
int main() 
{
    char str1[50], str2[50], copyStr[50];
    int cmp, len;
    printf("Enter first string: ");
    gets(str1);
    printf("Enter second string: ");
    gets(str2);
    len = strlen(str1);
    printf("\nLength of first string = %d", len);
    strcpy(copyStr, str1);
    printf("\nCopied string = %s", copyStr);
    strcat(str1, str2);
    printf("\nAfter Concatenation = %s", str1);
    cmp = strcmp(str1, str2);
    if(cmp == 0)
        printf("\nStrings are equal\n");
    else
        printf("\nStrings are not equal\n");
     return 0;
}
