# -WAP-to-generate-positive-Fibonacci-numbers
 WAP to generate positive Fibonacci number

 #include<stdio.h>
/* DOC
NAME:Dnyandev Nagre
DATE:10/10/2023
DISCRIPTION:WAP to generate positive Fibonacci numbers
SAMPLE INPUT:5
SAMPLE OUTPUT:0,1,1,2,3,5
DOC
 */

int main()
{
        //Take ip from user
        int first=0,sec=1,next=0,n;
        printf("enter the positive number :");
        //take and scan the ip from user
        scanf("%d",&n);
        //condition for the positive num
        if(n>0)
        {
                //print the first and sec num
                printf(" %d  %d",first,sec);
                //check condition for next is less than num
                while(next<=n)
                {
                        //for the fibonacci series
                        next=first+sec;
                        //assigning the value first to sec var
                        first=sec;
                        //sec to next assigning valve
                        sec=next;

                        //next is less than or equal to num
                        if(next<=n)
                        {
                                //print next number
                                printf(" %d",next);
                        }

                }
        }
        //check the condition for zero
        else if(n==0)
        {
                //print zero if con for true
                printf("0");
        }
        else
        {
                //print statement for invalid input
                printf("Invalid input");
        }
        return 0;
}

