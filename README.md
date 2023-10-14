# Valid_date
#include<stdio.h>
void main()
{

int day ;
printf("Enter your choice of days(1,2,3,4,5....31) ");
scanf("%d",&day);
int month ;
printf("Enter your choice (1,2,3,4,...12) of month");
scanf("%d",&month);
int year;
printf("Enter year ");
scanf("%d",&year);
if(month>=1 && month<=12 && day>=1 && day <=31 && year >=1000&& year<=9999  ){
printf("valid date \n");}
else
printf("Invalid  date");

switch(month)
{
case 1:case 3:case 5:case 7:case 8:case 10:case 12:
printf("no of days are 31 in this month");
break;
case 4:case 6:case 9:case 11:
printf("no of days are 30 in this month");
break;
case 2:
if(year%4==0)
{
printf("No of days are 28 in this month because it is not a leap year");
}
else
printf("No of days are 29 in this month because it is  a leap year");
}
}
