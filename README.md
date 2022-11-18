# GRADING-SYSTEM
/*** An IT Student Grading System  ****/

#include<stdio.h>
#include<conio.h>

void main()
{
int no, i;
float marks[10], per=0, total=0;
clrscr();
printf("Enter Marks: ");
scanf("%d",&no);
printf("Enter marks of %d subject: ",no);
for(i=0; i<no; i++)
{
scanf("%f",&marks[i]);
}
for(i=0; i<no; i++)
{
total=total+marks[i];
}
per=total/no;
printf("Percentage: %f % \n",per);
if(per>70) 
{
printf("A grade");
}
else if(per<69 && per>=60) 
{
printf("B grade");
}
else if(per<60 && per>=50)
{
printf("C grade");
}
else if(per<50 && per>=40) 
{
printf("D grade");
}
else if(per<40 && per>=0) 
{
printf("F grade");
}
getch();
}
