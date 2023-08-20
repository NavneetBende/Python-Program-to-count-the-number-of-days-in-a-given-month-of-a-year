# Python-Program-to-count-the-number-of-days-in-a-given-month-of-a-year

Number of days in a given month of a given year in  Python
Here, in this page we will discuss the program to find the number of days in a given month of a given year in python . Number of days in any month of a year can vary specifically in February as the cycle of leap year repeats in every 4 years when the year is leap February gives the count to 29 days but the when the year is not leap it gives count to 28 days and so no of days in a year varies from 365 to 366.

Number of days in a given month of a year in python
Method Discussed :
Method 1: Using if-else ladder.
Method 2 : Using Array
Method 1 :
Check if the given month is February. 
If True Check if the year is a year leap or not.
If year is a leap year Print 29 Days, Else Print 28 Days.
If Condition in Step 3 is False Check the month. 
Print the number of days assigned to specific Month.
Method 1 : Code in Python
Run
month = 12
year=2012
    
if((month==2) and ((year%4==0)  or ((year%100==0) and (year%400==0)))) :
    print("Number of days is 29");

elif(month==2) :
    print("Number of days is 28");

elif(month==1 or month==3 or month==5 or month==7 or month==8 or month==10 or month==12) :
    print("Number of days is 31");

else :
    print("Number of days is 30");
Output
Number of days is 31
Method 2 :
In this method instead of using if-else-if ladder or switch case, we use array.

Method 2 : Code in Python
Run
arr = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31 ]
month = 12
year=2012
    
if(month==2 and ((year%400==0) or ((year%100!=0) and (year%4==0)))) :
    print("Number of days is ", arr[month-1]+1)
    
else :
    print("Number of days is ", arr[month-1]);
Output
Number of days is 31
