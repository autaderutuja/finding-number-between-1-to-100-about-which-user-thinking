# finding-number-between-1-to-100-about-which-user-thinking
ask user to think about number between 1 to 100 and find that number by asking maximum 20 questions to user.
#include <stdio.h>

int main()
{ 
    char ans1;
    char ans2;
    char ans3;
int i,j;
    printf("think a number in mind between 1 to 100");
    for(j=0;j<=100;j=j+25)
{
    printf("\n are you thinking about number between %d to %d?",j+1,j+25);
    scanf("\n %c", &ans1);
    if(ans1=='y')
    {
        printf("\n number is even?");
        scanf("\n %c", &ans2);
        if(ans2=='y')
        {
         for(i=j+1;i<j+25;i=i+2) 
         {
           printf("\n are you thinking about %d ?", i); 
           scanf("\n %c", &ans3);
           if(ans3=='y'){
               printf("successfull...");
               break;
           }
         }
        }
        else
        {
          for(i=j;i<=25;i+=2) 
         {
           printf("\n are you thinking about %d ?", i); 
           scanf("\n %c", &ans3);
           if(ans3=='y'){
               printf("successful...");
               break;
           }
         }  
        }
    }
 }
    return 0;
}
