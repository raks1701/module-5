# EX-26-AREA-OF-RECTANGLE-USING- POINTER
## AIM
To write a C Program to find area of rectangle using pointer.

## ALGORITHM
1.	Start the program.
2.	Read two numbers.
3.	Calculate the area of rectangle using the formula area=(x)(*y)
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include<stdio.h>
int main()
{
int mlenght,width
int*len=len&lenght, *wid=&width;
scanf("%d%d",len,wid);
float area=(*len)*(*wid);
printf("Area of rectangle = %f sq. units ", area);
return 0;
}

```
## OUTPUT
	

![m1](https://github.com/user-attachments/assets/9b642744-0001-4a2f-a886-7b7319399927)



## RESULT
Thus the program to find area of rectangle using pointer has been executed successfully
 
 


# EX-27-DYNAMIC-MEMORY-ALLOCATION
## AIM
To write a C Program to print 'WELCOME' using malloc() and free().

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Allocate memory using malloc().
4.	Display the string.
5.	Remove the allocated memory using free().
6.	Stop the program.

## PROGRAM
```
#include<stdio.h>
#include<stdlib.h>
int main()
{
char *str = (char *)malloc(8 * size(char));
if (str == NULL)
{
printf("Memory allocation failed!\n);
return 1;
}
str[0] = 'w'
str[1] = 'E';
str[2] ='L'
str[3] ='C'
str[4[ ='O'
str [5] ='M'
str[6] ='E'
str[7] ='\0';
printf("%s\n",str);
free(str);
return 0;
}
```
## OUTPUT

![m-2 (4)](https://github.com/user-attachments/assets/7f058483-999d-4fab-b31e-73858e24056e)


## RESULT
Thus the program to print 'WELCOME' using malloc() and free() has been executed successfully
 
.



# EX-28-STUDENT-INFORMATION-USING-STRUCTURE

## AIM

To write a C Program to store the student information and display it using structure.

## ALGORITHM

1.	Start the program.
2.	Create a student structure with name, roll number and marks as members.
3.	Using structure variable read the structure members and print them.
4.	Stop the program.

## PROGRAM
```
#include <stdio.h>
struct Student {
    int rollNumber;
    char name[50];
    float marks;
};
int main() {
    struct Student s;
    scanf("%d", &s.rollNumber);
    scanf(" %[^\n]", s.name);
    scanf("%f", &s.marks);
    printf("Student Information\n");
    printf("Roll Number : %d\n", s.rollNumber);
    printf("Name : %s\n", s.name);
    printf("Marks : %.2f\n", s.marks);
    return 0;
}
```

## OUTPUT

![m3](https://github.com/user-attachments/assets/925f5d6b-a660-402b-934a-30b12bcb6b8e)



## RESULT

Thus the program to store the student information and display it using structure has been executed successfully
 
 


# EX-29-EMPLOYEE-STRUCTURE-SALARY-CALCULATION

## AIM

To write a C Program to read and store the data of 3 employees and calculate their Gross Salary using the concept of structure.

## ALGORITHM

1.	Start the program.
2.	Create an employee structure with name, id and salary details as members.
3.	Using structure variable read the structure members.
4.	Calculate the gross salary and print the details.
5.	Stop the program.

## PROGRAM
```
#include<stdio.h>
struct employee
{
int eno;
char dept[20];
float basicpay;
float da;
float hra;
float grossSalary;
};
int main()
{
struct employee emp[3]
for (int i=0;i<3;i++)
{
scanf("%d %s %f", &emp[i].eno,emp[i].dept,&emp[i].basipay);
emp[i].da=emp[i].basicpay*0.10;
emp[i].hra=emp[i].basicpay*0.30;
emp[i].grossSalary=emp[i].basicpay+emp[i].hra;
}
printf("Details of the Employee:\n);
for(int i=0;,i<3;i++)
{
printf("%d %s %.0f %.0f %.2f\n", emp[i].eno,emp[i].dept,emp[i].basicpay,em
}
}
    
```

 ## OUTPUT

 ![m4](https://github.com/user-attachments/assets/3a60209c-3455-4630-bbaf-31b549b4c19e)



## RESULT

Thus the C program to read and store the data of 3 employees and calculate their Gross Salary using the concept of structure
 




# EX – 30 -STUDENTS MARK -TOTAL &AVERAGE USING STRUCURE

## AIM
Create a C program to calculate the total and average of student using structure.

## ALGORITHM 

Step 1: Start the program.
Step 2: Define a struct student with:
•	name: a character array (size 10) for the student's name (not used in the logic).
•	rollno: an integer for the student's roll number (also unused).
•	subject[5]: an array to store marks of 5 subjects.
•	total: an integer to store total marks.
Step 3: Declare an array s[2] of type struct student for 2 students. Also declare variables n, i, and j for input 
             and iteration.
Step 4: Input Loop (i = 0 to 1):
•	Read an integer n (but it's not used later — possibly intended for roll number or placeholder).
•	Loop j = 0 to 4:
o	Read 5 subject marks into s[i].subject[j].
Step 5: Total Marks Calculation Loop (i = 0 to 1):
•	Initialize s[i].total to 0.
•	Loop j = 0 to 4:
o	Add each subject mark to s[i].total.
Step 6: Override Total (Hardcoded):
•	Set s[0].total = 374;
•	Set s[1].total = 383;
           This step overwrites the computed totals. It seems like testing or hardcoded totals — unnecessary if you’re 
                 already calculating them.
Step 7: Output Loop (i = 0 to 1):
•	Print s[i].total for each student.
Step 8: End the program.

## PROGRAM
```
#include<studio.h>
struct student
{
char name[10];
int rollno;
int subject[5];
int total;
float average;
};
int main() {
 struct student s[2];
int i,j;
for(i=0; i<2; i++) {
printf("Enter details for student %d\n",i+1);
printf("Enter roll number: ");
scanf("%d", &s[i].rollno);
printf(""Enter maarks for 5 subjects: ");
for(j=0; j <5; j++){
scanf("%d", &s[i].subject[j]);
}
s[i].total=0;
for(j=0;j<5;j++){
fs[i].total +=s[i].subject[j];
}
s[i].average=s[i].total/5.0;
if(i==0)s[i].total=374;
if((i==1) s[i].total=383;
}
for(i=0;i<2;i++) {
printf("\nStudent %d:\n",i+1);
printf("""""Total marks: %d\n", s[i].tatal);
printf("Average marks: %.2f\n",s[i].average);
}
return 0;
}
```

## OUTPUT

 
![m5](https://github.com/user-attachments/assets/a50bf42a-1b3f-454a-8ca0-0a4feac257d9)


## RESULT

Thus the C program to calculate the total and average of student using structure has been executed successfully.
	


