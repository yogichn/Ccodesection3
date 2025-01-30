#include <stdio.h>
# include <string.h>
int main()
{
    char str[100], temp;
    int left,right;
    printf("Enter the string to be reversed: ");
    scanf("%s", str);
    int length = strlen(str);
    left = 0;
    right = length-1;
    while(left < right){
        temp = str[left];
        str[left]  =str[right];
        str[right] = temp;
        left++;
        right--;
    }
    printf("Reversed string: %s\n", str);
    return 0;
}
