# LabWorkITWorkShop

## Python Worksheet 1

**Que 1. Calculate simple interest**
```
# this function is to find the simple Interest which is p*r*t  
def simpleInterest(p,r,t):
    return p*r*t/100;

# driver code takes input and call the function for simpleInterest     
p = int(input('Enter principal : '))
r = float(input('Enter rate: '))
t = int(input('Enter time : '))

# now finding and print the simple Interest where p,r,t are arguments  
print(f'the simple interest is {simpleInterest(p,r,t)} : ' )
```
test cases : 
```
 1 . principal = 1000 , rate = 2.5% , t = 5 yrs , simpleInterest = 125
 2 .principal = 1250 , rate = 3.3% , t = 8 yrs , simpleInterest = 330
** it can find simple interest for large number also  1e208 and more**
```



Ques 2. Ramesh’s basic salary is input through the keyboard. His dearness allowance is 40% of basic salary, and house rent allowance is 20% of basic salary. Write a program to calculate his gross salary.
```
# here we have have to find the gross salary after his DA and house rent allowance 
#basic salary 
s = float(input("enter the salary : "))
# DA
g = 0.4*s
#Rent  Allowance 
a = 0.2*s
#printing the gross salary : 
print(f'the gross salary is: {str(s+g+a)}')
```
test cases
```
 1 .basic salary - 2000 , Gross Salary - 3200 
 2 .basic salary - 10000 , Gross Salary - 16000
 3 .basic salary - 200000 , Gross Salary - 320000 
```

**3. The distance between two cities (in km.) is input through the keyboard. Write a program to convert and print this distance in meters, feet, inches and centimeters.**
```
# to find the distance in meter , feet , inch , centimeter
#  1 kilometer = 1000 meters
# 1 meter = 100 centimeters
# 1 meter = 3.28 feet
# 1 feet = 12 inches
# the above data i used to calculate the distance

# driver code
k = float(input("enter the distance : "))
# in meter
m = k*1000
# in feet
f = m*3.28084
# in centimeter
c = m*100
# in inches
i = f*12

# output :
print(f' the distance in meter is :  {m}')
print(" the distance in feet is : " + str(f))
print(" the distance in inch is : " + str(i))
print(" the distance in centimeter is : " + str(c))
```
 test cases
 ```
 1 . 400 km  400000 m , 1312336 feet , 15748032 inch , 40000000 cm 
 2 . 1 km 1000m , 3280.84 feet , 39370.08 inches , 100000 cm 
```


4. If the marks obtained by a student in five different subjects are input through the keyboard, find out the aggregate marks and percentage marks obtained by the student. Assume that the maximum marks that can be obtained by a student in each subject is 100.
```

#  here we have to find the Aggregate marks (total marks obtained) and percentage 

# here user should input marks <= 100 otherwise wrong output format  

# driver code  for inputs 
m1 = float(input("enter the marks for 1st Sub : "))
m2 = float(input("enter the marks for 2nd Sub : "))
m3 = float(input("enter the marks for 3rd Sub : "))
m4 = float(input("enter the marks for 4rt Sub : "))
m5 = float(input("enter the marks for 5th Sub : "))

# finding total marks (aggregate)
ag = m1+m2+m3+m4+m5
print("Aggregate marks is : " + str(ag))
# finding percentage 
print("percentage marks is : " + str(ag*100/500))
```
test cases :
```
# 1 . sub1 = 77 , sub2 = 75 , sub3 = 84 , sub4 = 90 , sub5 = 97 , Aggregate = 423 , percentage = 84.6% 
# 2 .  sub1 = 94 , sub2 = 50 , sub3 = 79 , sub4 = 86 , sub5 = 78 , Aggregate = 387 , percentage = 77.4% 
```



5. Temperature of a city in Fahrenheit degrees is input through the keyboard. Write a program to convert this temperature into Centigrade degrees.
```

# converting Fahrenheit to centigrade 

# Driver code 
t = float(input("enter the temperature in Fahrenheit "))
# formula f = (9/5)*c + 32 
c = (t-32)*5/9
print("the temperature in Centigrade is " + str(c) + "°C")
```
 test cases : 
```
# 1 . fahrenheit is - 99.0 ,  Centigrade is -  37.22°C
# 2. fahrenheit is - 104.5 , Centigrade is - 40.277 °C
```


6. The length & breadth of a rectangle and radius of a circle are input through the keyboard. Write a program to calculate the area & perimeter of the rectangle, and the area & circumference of the circle. 
```
# to find area and perimeter(circumference) of the rectangle and circle

# Driver Code 
# length input 
l = float(input("enter the length of rectangle : "))
# breadth input
b = float(input("enter the breadth of rectangle : "))
# radius input 
r = float(input("enter the radius of the circle : "))

# output section 
print(" the perimeter of rectangle is : "+ str(2*(l+b)))
print(" the area of rectangle is : "+ str(l*b))
print("the Circumference of the circle is : "+ str(2*22*r/7))
print("the area of the circle is : "+ str(22/7*(r**2)))
```

 test cases :
```
# 1. length : 24 unit , breadth : 10.5 unit , radius :  7 unit, perimeter rectangle : 69 unit , area rectangle : 252 unit square   , circumference circle : 44 unit , area circle : 154 unit square,
# 2 . length : 10 unit , breadth : 10 unit , radius : 10 unit , perimeter rectangle : 40 unit , area rectangle : 100 unit square , circumference circle : 62.85 , area circle : 314.285 unit square ,
```


7. Two numbers are input through the keyboard into two locations C and D. Write a program to interchange the contents of C and D.
``` 
# interchange aur swap the content 
# Driver code : 
# input x 
x = input('Enter value of x: ')
# input y 
y = input('Enter value of y: ')
#  now swapping with help of temp variable which work as temporary variable to store data and help in swapping 
temp = x
x = y
y = temp
print(f' x is {x} and y is {y}')
```

 test cases :
```
#  1 . x = 5 , y = 6  after swap x = 6 , y = 5 
#  2 . x = 15.6 , y = 6  after swap x = 6 , y = 15.6
#  3 . x = Ashish , y = 6  after swap x = 6 , y = Ashish 
```


8. If a five-digit number is input through the keyboard, write a program to calculate the sum of its digits. (Hint: Use the modulus operator ‘%’)
``` 

# here  calculating the sum of the digit of the integers numbers only not for float and double , as mentioned 

# driver code 
# input of the number it should be only number of integer type 
n = int(input("enter the number : "))

# here using % to find sum of every digit and dividing number by 10 till it reaches 0 
sum = 0
while n > 0:
   sum += n%10
   n = int(n/10)
print("the sum is : "+ str(sum))
```
 Test cases :
```
#  1. the number is : 2345 , sum = 14 
#  2. the number is : 12345 , sum = 15
#  3. the number is : 121.4 , output : invalid input 
```


9.If a five-digit number is input through the keyboard, write a program to reverse the number. 
```
# reversing the number 
# driver code 
# input number only as given 
n = int(input("enter the number : "))
# here using while loop and reverse = 0 and incresing reverse in every step and multiplying with 10 to get the tenth place in first step and so on 
reverse = 0
while n > 0:
    reverse = reverse*10 + n%10
    n = int(n/10)
# printing the reverse 
print("the reverse numbers is : "+ str(reverse))
```
 test cases
```
# 1 . number = 12345  , reverse = 54321
# 2 . number = 111 , reverse = 111
# 3 . number = Ashish  , output = error invalid input  
```


10.If a four-digit number is input through the keyboard, write a program to obtain the sum of the first and last digit of this number. 
```
# sum of first and last digit of integer number ,
# number can be of any length
n = int(input("enter the number : "))
# using % for finding the last and then divinding the number till it become greater than 10 or store the number on before  every divide of 10 and add the number stored
sum = n % 10
while n > 0:
    b = n % 10
    n = int(n/10)
sum += b
print("the sum of last and first  is " + str(sum))
```
 test cases :
 ```
# 1 . number = 12345 , sum = 6
# 2 . number = 99999 , sum = 18
# 2 . number = Ashish , output : invalid input (error)
```


11.A cashier has currency notes of denominations 10, 50 and 100. If the amount to be withdrawn is input through the keyboard in hundreds, find the total number of currency notes of each denomination the cashier will have to give to the withdrawer.
``` 

# here we are finding the minimum number of notes required to withdraw
# driver code 
# input we will not consider values in ones place   
n = int(input("enter the cash you want to withdraw : "))
count = 0
if n > 100 : 
    count += n//100
    n = n%100
elif n> 50 : 
    count += n//50
    n = n%50
else : 
    count += n//10
print(f'the number of notes are : {count}')
```
test cases :
```
#  1 . amount = 1111 , notes = 11
#  2 . amount = 54 , notes = 1
#  3 . amount = 100 , notes = 1
```



12.If the total selling price of 15 items and the total profit earned on them is input through the keyboard, write a program to find the cost price of one item.
``` 
# finding the cost price of the each item when there are 15 item 
# given selling price and profit earned 
# driver code 
n = int(input("enter the selling price : "))
p = int(input("enter the profit gained : "))
# as cost price will be selling price - profit and for each item divide by total items
print(f'the cost price of each item is : {(n-p)/15} ')
```
test cases :
```
#  1. SP = 1200 , profit = 200 , cost price per item = 66.67
#  2. SP = 1208 , profit = 9  , cost price per item = 79.93
#  3. SP = 1645 , profit = 33 , cost price per item = 107.46
```



13.If a five-digit number is input through the keyboard, write a program to print a new number by adding one to each of its digits. For example if the number that is input is 12391 then the output should be displayed as 23402.
``` 

# here we have to find th new number which is 1 added to every digit of the number if the digit is 1 it become 2 and if it is 9 it becomes 0 and so on and 1 doest not carry over
# driver code  
# taking input 
n = int(input("enter the number  : "))
# here new is the  number which  is  used  to stored the intermediate of the reversed output  
new = 0
while n>0:
    # here n%10 to find the digit and 1 is added and then %10 to insure that number should not increase more than 9 
    new = new*10 + (n%10 + 1)%10
    n = n//10

n = 0 
# now converting the number i.e reversing the new to get the desired number 
while new>0 :
    n = n*10+new%10
    new = new//10
print(f'the new number is : {n}')
```
test cases :
```
# 1 . number = 12345678 , new number = 23456789
# 2 . number = 100 , new number = 211
# 3 . number = 99999 , new number = 0
```



14.Write a program to round off an integer i to the next largest multiple of another integer j . For example, 256 days when rounded off to the next largest multiple divisible by a week results into 259.
``` 

# generalising the question to find the next larger multiple of the given number by and another number  
# drive code 
# input number whose nearest largest multiple to be found 
n = int(input("enter the number i : "))
# input the number whose multiple is the nearest to the above number : 
p = int(input("enter the integer j "))
# first the quotient and adding 1 and then multiplying to find the next larger 
div = n//p 
n = (div+1)*p
print(f'the next largest multiple is : {n}')
```
 test cases 
```
# 1 . i = 546 , j = 7 , next multiple of j near i is : 553
# 2 . i = 356 , j = 8 , next multiple of j near i is : 360
# 3 . i = 211 , j = 11 , next multiple of j near i is : 220
# 4 . i = 121 , j = 11 , next multiple of j near i is : 121
# if i%j == 0 then it will also give the next multiple
```


15.Two variables a and b contain values 10 and 20. Write a program to interchange the contents of a and b without using a third variable.

```

# there are many method for the swap without variable , one of the method is shown below : here we can take any value for a and b 
# driver code
# takes input  x,y to swap
x = input("enter the variable ")
y = input("enter the variable ")
# equate at one go
x, y = y, x
print(f'the swap value of x = {x} and y : {y}')
```
test cases : 
```
#  1 . x = 5 , y = 6  after swap x = 6 , y = 5 
#  2 . x = 15.6 , y = 6  after swap x = 6 , y = 15.6
#  1 . x = Ashish , y = 6  after swap x = 6 , y = Ashish 
```


16.Write a program to find out how many days and how many weeks have passed between the dates 01/01/92 to 31/05/92. Also find out how many days could not get evened out into weeks.
```
# here we have given inputs and to find the number of days between them
# d1 and d2 are the dates  
d1 = "01/01/92"
d2 = "31/05/92"
# finding months , days , years to figure where they are in the calender 
y1 = int(d1[-2:])
y2 = int(d2[-2:])
m1 = int(d1[4:5])
m2 = int(d2[4:5])
da1 = int(d1[0:2])
da2 = int(d2[0:2])
days = 0
weeks = 0
# adding days to totalDays which was initialise to zero according to the months 
while m1 < m2:
    if m1 % 2 == 1:
        days += 31
    elif m1 == 2:
        days += 29
    else:
        days += 30
    m1 += 1
# adding number of days left 
days += da2
# no of weeks are just totalDays // 7 
weeks = int(days/7)
# days left to even up to week is totalDays%7
daysLeft = days % 7
print(
    f'number of days between them is : {days} \nnumber of weeks are : {weeks} \nthe days which left to get evened in the week is : {daysLeft}')
```
test cases : only one test cases as given
```
# 1 .  d1 = "01/01/92" and d2 = "31/05/92" , Days = 152 , in Weeks = 21 , evenedDays  = 5
```


## Python Worksheet 2


QUESTION 1. If cost price and selling price of an item is input through the keyboard, write a program to determine whether the seller has made profit or incurred loss. Also determine how much profit he made or loss he incurred.

```
# program to find the gain and loss according to the input SP and CP 
# driver code  
# taking SP 

n1 = int(input("enter the selling price : "))

# taking input CP

n2 = int(input("enter the cost price : "))

# checking for gain and loss or (no gain and no loss)

if n1-n2 > 0 : 
    print("seller has made Profit of : ", (n1-n2))
elif n1-n2 < 0 : 
    print("seller has made loss of ", (n2-n1))
else : 
    print("no loss no gain ")

```
 test cases 
```
# 1 . SP = 140  , CP = 80 , Output = seller has made Profit of :  60
# 2 . SP = 80  , CP = 140 , Output = seller has made loss of  60
# 3 . SP = 80  , CP =  80 , Output = no loss no gain
```


QUESTION 2. Any integer is input through the keyboard. Write a program to find out whether it is an odd number or even number.


```
# program to find whether given input is odd or even 
# driver code
 
# input
n1 = int(input("enter the number : "))

# checking with % for even and odd if divisible by 2 even otherwise odd 
if n1%2 : 
    print("odd")
else :
    print("even")
```

 test cases : 
```
# 1 . number =  4 , output = even  , 
# 2 . number =  5 , output = odd  , 
# 3 . number =  Ashish , output = error (invalid literal ) , 

```


QUESTION 3. Any year is input through the keyboard. Write a program to determine whether the year is a leap year or not. 

```
# program to find whether leap year or not 

# driver code 

# input year 
n1 = int(input("enter the year : "))
# as leap year is either divisible by 400  or if not by 400 then by 4 but not by 100 

if n1%400 == 0 : 
    print("Leap Year")
elif n1%4==0 :
    if n1%100 == 0 :
        print("Not a Leap Year")
    else :
        print("Leap Year")
else : print("Not a Leap Year")

```
test code :
```
#  1 . year = 1200 , output = Leap Year
#  2 . year = 1900 , output = Not a Leap Year
#  3 . year = 2021 , output = Not a Leap Year
```


QUESTION 4. According to the Gregorian calendar, it was Monday on the date 01/01/1900. If any year is input through the keyboard write a program to find out what is the day on 1st January of this year.


```

# we have to take input and find the day of the first Date of the year


# day is the function which determine the day

# here we know that numbers of days and after every seven day is monday using that fact i find the total number of days in between the years and then modulo 7 to find the day .. 

# we find the day for n > 1900 and not less than 1900 

def day(n):
    ref_year = 1900
    leap = 0
    diff = n - ref_year
    while ref_year < n:
        if ref_year % 100 == 0:
            if ref_year % 400 == 0:
                leap += 1
        else:
            if ref_year % 4 == 0:
                leap += 1
        ref_year += 1
    total_days = (diff - leap) * 365 + leap * 366
    p = total_days % 7
    # as user can input n less than 1900 so used abs and modulo to find the day
    if p == 0:
        print("Monday")
    elif p == 1:
        print("Tuesday")
    elif p == 2:
        print("wednesday")
    elif p == 3:
        print("Thusday")
    elif p == 4:
        print("Friday")
    elif p == 5:
        print("Saturday")
    else:
        print("Sunday")



# driver code will be :
# input of year :

n = int(input("enter the year : "))

# if n< 1900 before the year 1900 can't be determine

if n < 1900 : 
    print("before the year 1900")
# calling function to find the day :
else : 
    day(n)
```
 test cases :
```
#  1 . year : 1900  , day :  Monday
#  2 . year : 2021 , day :  Tuesday
#  3 . year : 1899 , day : before the year 1900 can't be determine
#  4 . year : 2000 , day :  Saturday
```





QUESTION 5. Write a program to find the greatest of the three numbers entered through the keyboard.

```
# for find the maximum of three number

# here MAX_NUMBER return the maximum of the two number  
def MAX_NUMBER(a,b): 
    if a>=b : return a 
    else : return b 


# driver code 

# input three integers  
a = int(input("enter the number1 : "))
b = int(input("enter the number2 : "))
c = int(input("enter the number3 : "))

# using MAX_NUMBER function which return max of two number using that for comparing first two then next two numbers
print(MAX_NUMBER(a,MAX_NUMBER(b,c)))
```
 test cases : 
```
# 1 . a = 1 , b = 1 , c = 1 , MAX_NUMBER = 1 
# 2 . a = 1 , b = 2 , c = 3 , MAX_NUMBER = 3
# 3 . a = 4 , b = 1 , c = 1 , MAX_NUMBER = 4  
```





QUESTION 6. A five-digit number is entered through the keyboard. Write a program to obtain the reversed number and to determine whether the original and reversed numbers are equal or not.

  
```
# this program first reverse and then check palindrom for the reverse number and the actual numbers 


# this function is to return the reverse number of the current number
def Reverse(n1) : 
    res = 0
    while n1 > 0:
        res = (res*10) + (n1 % 10)
        n1 = int(n1/10)
    return res 


# driver code 

# take input of the number 
n1 = int(input("enter the number : "))

# now reverse the number
res = Reverse(n1)


# check whether the reverse and original numbers were same or not and print the result according to that condition 
if res == n1 :
    print("yes palindrom ")
else:
    print("No palindrom ")

```
test cases : 
```
# 1 : n1 = 1221  reverse = 1221 , yes Palindrom 
# 2 : n1 = 12212  reverse = 21221 , no Palindrom 
# 3 : n1 = 1111  reverse = 1111 , yes Palindrom 
```


QUESTION 7. Given three points (x1, y1), (x2, y2) and (x3, y3), write a program to check if all the three points fall on one straight line. y = mx + C here m is slope and can be calculated (Change in Y) / (Change in X).

```

# taking input as three points and finding whether they have equal slope at any combinations of  two points if yes then lie on the same line otherwise not on same line 

# drivers code :


# taking input as three points
 
x1, y1 = input("Enter the x1 point : "), input("Enter the y1 point : ")
x2, y2 = input("Enter the x2 point : "), input("Enter the y2 point : ")
x3, y3 = input("Enter the x3 point : "), input("Enter the y3 point : ")


# finding there slopes for each possible combinations : 
m1 = float((float(y3) - float(y2))/(float(x3) - float(x2)))
m2 = float((float(y2)-float(y1))/(float(x2)-float(x1)))
m3 = float((float(y3 )- float(y1))/(float(x3) - float(x1)))


# checking there slopes : 
if m1 == m2:
    if m1 == m3:
        print("the point lies on same line . ")
    else:
        print("the point does not lies on the same line . ")
else:
    print("the point does not lies on the same line .")
    
```


test cases : 
```
# 1 . (x1,y1) = (1,1 ) , (x2,y2) = (2,2) , (x3,y3) = (3,3) output:   the point lies on same line .
# 2 . (x1,y1) = (1,0 ) , (x2,y2) = (2,1) , (x3,y3) = (3,3) output:   the point does not lies on same line .

```


QUESTION 8. Given the coordinates (x, y) of a center of a circle and it’s radius,write a program which will determine whether a point lies inside the circle, on the circle or outside the circle.


```
# for finding whether the point lie on , inside or outside of the circle , 
# given radius and coordinate of the centre and given a point find the output 


# driver code 


#  for taking input of the centre of the circle 
x1,y1 = float(input("enter the x coordinate of centre of circle : ")),float(input("enter the y coordinate of centre of circle : "))


# for the radius of the circle : 
r = float(input("enter the radius of the circle : "))

# for taking the coordinate of the point of which we have find whether it lie on , inside or outside of the circle 
x , y = float(input("enter the x coordinate : ")),float(input("enter the y coordinate : "))

# the concept is i will find the distance of the point from the centre of the circle if distance  is equal to the radius then it will lie on the circle and if greater then outside of the circle and if less then inside of the circle 
z = float((float(x1-x))**2 + (float(y1-y))**2)
disFromCircle = float(z ** 0.5)

# checking for the point 
if r < disFromCircle : 
    print(f' ({x},{y}) lies outside circle ')
elif r == disFromCircle : 
    print(f' ({x},{y}) lies on circle ')
else : 
    print(f' ({x},{y}) lies inside of circle ')
 ```   


test cases : 
```
#  1 . (x,y) = (0,0) , r = 5 , (x1 ,y1) = (0,4) , output : lies inside the circle
#  2 . (x,y) = (0,0) , r = 4  , (x1 ,y1) = (0,4) , output : lies on the circle
#  3 . (x,y) = (2,3) , r = 4  , (x1 ,y1) = (12 , 13)  , output : lies outside the circle

```




QUESTION 9. A library charges a fine for every book returned late. For first 5 days the fine is 50 paise per day, for 6-10 days fine is one rupee per day and above 10 days fine is 5 rupees per day. If you return the book after 30 days your membership will be cancelled. Write a function to accept the number of days the member is late to return the book and display the fine or the appropriate message.


```
# below program is to find the fine charges by the library on late submission 

# driver code 

# input of number of days of late submission :  
n = int(input("enter the number of days you are late "))

# sum will store the fine charged
sum = 0.0
if n > 30 : 
    print("your membership is cancelled ")
elif n <= 0 : 
    # if n is less than or zero then no charge fine 
    print("No charge fined ")
else : 
    # here we are adding charges and reducing the days according to the range of charges
    if n > 10 : 
        sum += (n-10)*5
        n = 10;
    if n> 5 : 
        sum += (n-5)
        n = 5
    if n>0: 
        sum += n*0.5
    print(f'the fine is {sum} rupees')

```

 test cases : 
```
#  1 . n = 3 , charge = 1.5
#  2 . n =  7, charge = 4.5
#  3 . n =  18, charge = 47.5
#  4 . n =  0 , charge = No charge fined
#  5 . n = 31 , charge = your membership is cancelled 
```





QUESTION 10. write a program to decide the division of a student as following rules.
(1) There are 5 paper in each semester
(2) Maximum marks may vary for each paper
(3) if below then 40% for any two paper result is fail.
(4) if below then 40% for any paper result paper due.
(5) if total % below 33% result fail.
(6) if total % between 33% to 45% result third division.
(7) if total % between 45% to 60% result second division.
(8) if total % between 60% to 70% result first division.
(9) if total % above 70% result PASS WITH HONS. 

 
```
# program to define the division of the student

# driver code : 

# as maximum marks for one subject can change so we can ask user to input the total marks of the each subject also 
marks1 = input("Enter the marks of first subject : ")
total1 = input("Total number of first subject : ")
marks2 = input("Enter the marks of second subject : ")
total2 = input("Total number of second subject : ")
marks3 = input("Enter the marks of third subject : ")
total3 = input("Total number of third subject : ")
marks4 = input("Enter the marks of fourth subject : ")
total4 = input("Total number of fourth subject : ")
marks5 = input("Enter the marks of fifth subject : ")
total5 = input("Total number of fifth subject : ")

# now calculating the whether subject is due or not as if it less than 40 percent of total marks of each subject
due = 0 
if float(float(marks1)/float(total1)) <= 0.4 :
    due+=1
if float(float(marks2)/float(total2)) <= 0.4:
    due+=1
if float(float(marks3)/float(total3)) <= 0.4: 
    due+=1
if float(float(marks4)/float(total4)) <= 0.4 : 
    due+=1
if float(float(marks5)/float(total5)) <= 0.4  : 
    due+=1
if due >=2 : 
    print("Fail")
    print(f'{due} dues subjects')

# now print out the final Remark
total  = total1+total2+total3+total4+total5
agr = marks1+marks2+marks3+marks4+marks5

if due < 2 : 
    if float(float(agr)/float(total)) < 0.33 : 
        print("Final Remark : Fail");
    elif float(float(agr)/float(total)) < 0.45 : 
        print("Final Remark : Third Division")
    elif float(float(agr)/float(total)) < 0.6 : 
        print("Final Remark : Second Division")
    elif float(float(agr)/float(total)) < 0.7 : 
        print("Final Remark : First Division")
    else : 
        print("Final Remark : PASS WITH HONS") 
    
```

 TEST CASES : 
```
# 1 .
# Enter the marks of first subject : 10
# Total number of first subject : 15
# Enter the marks of second subject24
# Total number of second subject30
# Enter the marks of third subject45
# Total number of third subject60
# Enter the marks of fourth subject32
# Total number of fourth subject60
# Enter the marks of fifth subject67
# Total number of fifth subject80
# Final Remark : First Division

# 2 . 
# Enter the marks of first subject : 26
# Total number of first subject : 50
# Enter the marks of second subject : 12
# Total number of second subject : 40
# Enter the marks of third subject : 24
# Total number of third subject : 60
# Enter the marks of fourth subject : 45
# Total number of fourth subject : 70
# Enter the marks of fifth subject : 45
# Total number of fifth subject : 80
# Fail
# 2 dues subjects

```

QUESTION 11. Write a function to find the factorial value of any number entered through the keyboard.


```
# program to find the factorial of the given number 

# driver code 

# intout the number
num = int(input("Enter a number: "))

# initialise the factorial to be 1 
factorial = 1

# for different condition fatorial is found out 

if num < 0:
    print("Sorry, factorial does not exist for negative numbers")
elif num == 0:
    print("The factorial of 0 is 1")
else:
    for i in range(1,num + 1):
        factorial = factorial*i
    print("The factorial of",num,"is",factorial)

```

 TEST CASES : 
```
# 1 . n = 10  , output = 3628800
# 2 . n = 0 , output = 1
# 3 . n =  -5 , output = Sorry, factorial does not exist for negative numbers
```

QUESTION 12. Write a program for a matchstick game being played between the computer and a user. Your program should ensure that the computer always wins. Rules for the game are as follows:
    - There are 21 matchsticks.
    - The computer asks the player to pick 1, 2, 3, or 4 matchsticks.
    - After the person picks, the computer does its picking.
    - Whoever is forced to pick up the last matchstick loses the game.

```
#  program to write the game of pick up match stick , the one who picks as last losses 

# total number of sticks at the begining of the game
sticks = 21

# giving instruction about the game 
print ("There are 21 sticks, you can take 1-4 number of sticks at a time.")
print ("Whoever will take the last stick will win")

# using infinite loop for picking up sticks as number of chances are not fixed 
# using break  for breaking the loop and
while True:
    # it will print the sticks left 
    print( "Sticks left: " , sticks)
    #  ask user to pick up stick 
    sticks_taken = int(input("Take sticks(1-4):"))
    if sticks == 1:
        print( "You took the last stick, you loose")
        break
    #  checking whether the user has taken correct number of sticks or otherwise ask him again to pick up stick 
    if sticks_taken >= 5 or sticks_taken <= 0:
        print( "Wrong choice")
        continue
    
    # computer should always wins which means computer has to pick up stick  according to the users so computer can not choose  random sticks 
    
    # so we use the algorithm where we sum up  number of sticks user chooses and computer to be 5 in this way they will have four changes to choose and user will forced to choose the last one as 5*4 = 20 so 1 is left always 
    p = 5 - sticks_taken
    print (f'Computer took :  {p} \n')
    sticks -= 5
  ```  

 test cases 
```
# 1 . user = 1 , computer = 4 , user = 2 , computer = 3 , user = 4 , computer = 1 , user = 2 , computer = 3 , user  = 1 , user losses 
# 2 . user = 2 , computer = 3 , user = 4 , computer = 1 , user = 2 , computer = 3 , user = 4 , computer = 1 , user  = 1 , user losses 
```


QUESTION 13. Write functions to calculate the binary, octal, hexadecimal  equivalent of the entered decimal number.


```
# program is to find the binary , octal , hexadecimal  of the decimal number

# for binary number we divide it dy 2 continuously till it reaches 1 will give the binary equivalent code 
def binary(n):
    if n > 1:
        binary(n//2)
    print(n % 2, end='')

# for octal number we divide it dy 8 continuously till it reaches 0 and then append the result in an array  and then use the octal number
def octal(n):
    result = list()
    while n:
        res = n % 8
        n = n // 8
        result.append(res)
        # here result array result[::-1] is used to slice and -1 is used to reverse the array , which will be the octal number 
    return result[::-1]



# hexadecimal function for the decimal number n 
def hexadecimal(n):
    i = 0
    # here making an array for the storing the numbers 
    hexdecnum = []
    while n != 0:
        rem = n % 16
        # storing the NUMBER 0,1,2,3,4,5,6,7,8,9 in ascii value 
        if rem < 10:
            rem = rem+48
        else:
            # storing the character A,B,C,D,E,F in ascii value 
            rem = rem+55
            # chr is used to convert the digits in their ascii values 
        rem = chr(rem)
        hexdecnum.insert(i, rem)
        i = i+1
        n = int(n / 16)
        # printing the NUMBER in hexadecimal form 
    print("\nEquivalent Hexadecimal Value is: ")
    i = i-1
    while i >= 0:
        print(end=hexdecnum[i])
        i = i-1
    print()


# Driver Code

# input of decimal number :

dec = int(input("Enter an integer: "))
print("Binary number is : ")
# calling functions for binary
binary(dec)
print()
# calling functions for octal
octal(dec)
ans = octal(dec)
if dec == 0:
    print("Octal number is : ")
    print(0)
else:
    print("Octal number is : ")
    for i in ans:
        print(i, end=" "),
if dec == 0:
    print("\nEquivalent Hexadecimal Value is: ")
    print("0000")
else:
    # calling functions for hexadecimal
    hexadecimal(dec)
  ```  

test cases : 
```
# 1. 
# Enter an integer: 1234
# Binary number is :
# 10011010010
# Octal number is :
# 2 3 2 2
# Equivalent Hexadecimal Value is:
# 4D2


# 2. 
# Enter an integer: 9999
# Binary number is : 
# 10011100001111
# Octal number is :
# 2 3 4 1 7
# Equivalent Hexadecimal Value is:
# 270F
```

QUESTION 14. Write a program to print all prime numbers from 1 to 300.


```
# I am generalising the question and finding the prime number from 1 to n in o(log(n)) which is the fastest to find prime numbers . i am using function primeNumber() function which create an array to find the prime number and it takes a number from 2 and marks all the multiple false as they are not prime similarly  for 3 and so on ... 

def primeNumber(n) : 
    # array to store the prime number
    isPrime = [True for i in range(n+1)]
    # starting from the first prime number
    i = 2 
    # as it is a fact to know that factors of number lie under sqrt(n) and we can find the other factors if a*b = c , here a is under atmost sqrt(c) and b is above and equal to sqrt(c) so if we have a then we can find c / a to find b so we need loop till sqrt of n to discover all the non prime and whatever left is prime .   
    while i*i <= n : 
        if isPrime[i] :
            # finding factors of prime till that number as they are not prime and dismissing them .. 
            for j in range(i**2 , n+1 , i) : 
                isPrime[j] = False
        i += 1
    isPrime[0] = False
    isPrime[1] = False
    # printing the all the prime factors 
    for j in range(n+1): 
        if isPrime[j]: 
            print(j,end=' '),


# driver code 
# taking n as the range to find prime number from 1 to N (both inclusive )
n = int(input("enter the number up to which you want to find the prime numbers : "))
if n==0 or n==1 : 
    print("no prime number till now ")
else : 
    primeNumber(n)
```

constraint 
```
    # n <= 1e7 very easily in O(log(1e7)) = O(7) which is very fast but if we take O(1) = 1ms then 7ms which is very fast.
    # it can find greater than that but the we don't have array larger than 1e7 or 1e8 that why it make it difficult for it . otherwise if we use normal prime finding function which runs for every i in the loop  to check it is divisible or not and then give result then it will take 1e7 ms which either not possible or it will take  2.7 hrs to completely find that .. 
```

some test cases 
```
# 1. for 1 to 1000 : 2 3 5 7 11 13 17 19 23 29 31 37 41 43 47 53 59 61 67 71 73 79 83 89 97 101 103 107 109 113 127 131 137 139 149 151 157 163 167 173 179 181 191 193 197 199 211 223 227 229 233 239 241 251 257 263 269 271 277 281 283 293 307 311 313 317 331 337 347 349 353 359 367 373 379 383 389 397 401 409 419 421 431 433 439 443 449 457 461 463 467 479 487 491 499 503 509 521 523 541 547 557 563 569 571 577 587 593 599 601 607 613 617 619 631 641 643 647 653 659 661 673 677 683 691 701 709 719 727 733 739 743 751 757 761 769 773 787 797 809 811 821 823 827 829 839 853 857 859 863 877 881 883 887 907 911 919 929 937 941 947 953 967 971 977 983 991 997

# (asked for ) 1 to 300 : 2 3 5 7 11 13 17 19 23 29 31 37 41 43 47 53 59 61 67 71 73 79 83 89 97 101 103 107 109 113 127 131 137 139 149 151 157 163 167 173 179 181 191 193 197 199 211 223 227 229 233 239 241 251 257 263 269 271 277 281 283 293 
```


15. Write a program to produce the following pattern where number of line entered by keyboard:

#### *
#### **
#### ***
#### ****
#### ___________________
####    *
####   * *
####  * * *
#### * * * *
#### ____________________ 
#### ****
#### ***
#### **
#### *
#### ____________________
#### ****
#### ***
#### **
#### *
#### _____________________

i.e. if input is 7
#### *
#### **
#### ***
#### ****
#### ***
#### **
#### *
& if input is 8
#### *
#### **
#### ***
#### ****
#### ****
#### ***
#### **
#### *
i.e. if input is 7
####        *
####     **
####   ***
#### ****
####   ***
####     **
####       *
& if input is 8
####       *
####     **
####   ***
#### ****
#### ****
####   ***
####     **
####       *
i.e. if input is 7
 
####       *
####     ***
####   *****
#### *******
####   *****
####     ***
####       *
& if input is 8 
####       *
####     ***
####   *****
#### *******
#### *******
####   *****
####     ***
####       *

#### 12345
#### 6789
#### 012
#### 34
#### 5

 i.e. if input is 5
####     1
####   234
#### 56789
####   012
####     3

 & if input is 6
####   1
####  234
#### 56789
#### 01234
####  567
####    8

#### 0
#### 10
#### 010
#### 1010

```

# print statements and printing the pattern
import math as mt

# function for printing lines

def PrintLine(n):
    print()
    for i in range(n+1):
        print("_", end="_")
    print()


# function for printing the first Pattern
# *
# * *
# * * *
# * * * *
# * * * * *

def FirstPattern(n):
    # outer loop to handle number of n
    # n in this case

    for i in range(0, n):

        # inner loop to handle number of columns
        # values changing acc. to outer loop
        for j in range(0, i+1):

            # printing stars
            print("* ", end="")

        # ending line after each row
        print("\r")
    PrintLine(n)


# for second Pattern :
#    *
#   * *
#  * * *
# * * * *

def SecondPattern(n):
    # number of spaces
    k = n - 1

    # outer loop to handle number of n
    for i in range(0, n):

        # inner loop to handle number spaces
        # values changing acc. to requirement
        for j in range(0, k):
            print(end=" ")

        # decrementing k after each loop
        k = k - 1

        # inner loop to handle number of columns
        # values changing acc. to outer loop
        for j in range(0, i+1):

            # printing stars
            print("* ", end="")

        # ending line after each row
        print("\r")
    PrintLine(n)


# for third Pattern
# ****
# ***
# **
# *

def ThirdPattern(n):
    # loops goes to n+1 as we need at least one star at the end of the pattern
    for i in range(n+1):
        j = 0
        # starts will reduce at each loop 
        while j < (n-i):
            print("*", end=" ")
            j += 1
        print()
    PrintLine(n)


# Fourth Pattern
# ****
#   ***
#     **
#       *
def FourthPattern(n):
    for i in range(n):
        # as loop will  print 2 times the space to get the tilt shape
        for j in range(0, 2*i):
            print(" ", end="")
        for j in range(n, i, -1):
            print("*", end="")
        print()
    PrintLine(n)

# Fifth Pattern
# *
# **
# ***
# ****
# ***
# **
# *


def FifthPatternO(n):
    n = mt.ceil(n/2)
    # this loop  print the first half 
    for i in range(0, n):
        for j in range(0, i + 1):
            print("* ", end='')
        print("\r")
    # second half starts
    for i in range(n, 0, -1):
        for j in range(0, i - 1):
            print("* ", end='')
        print("\r")
    PrintLine(n)


# Fifth Pattern 
# & if input is 8
# *
# **
# ***
# ****
# ****
# ***
# **
# *

def FifthPatternE(n):
    n = mt.ceil(n/2)
    # this loop  print the first half 
    for i in range(0, n):
        for j in range(0, i + 1):
            print("* ", end='')
        print("\r")
    # second half starts
    for i in range(n+1, 0, -1):
        for j in range(0, i - 1):
            print("* ", end='')
        print("\r")
    PrintLine(n)

# Sixth Pattern 
# i.e. if input is 7


#        *
#     **
#   ***
# ****
#   ***
#     **
#       *

def SixthPatternO(n):
    n = mt.ceil(n/2)
    for i in range(n):
        for j in range(2*n - i, i, -1):
            print(" ", end="")
        for j in range(0, i):
            print("*", end="")
        print()
    for i in range(n):
        for j in range(0, 2*i):
            print(" ", end="")
        for j in range(n, i, -1):
            print("*", end="")
        print()
    PrintLine(n)

# sixth Pattern
# & if input is 8


#       *
#     **
#   ***
# ****
# ****
#   ***
#     **
#       *

def SixthPatternE(n):
    n = mt.ceil(n/2)
    for i in range(n):
        for j in range(2*n - i, i, -1):
            print(" ", end="")
        for j in range(0, i):
            print("*", end="")
        print()
    for i in range(n):
        for j in range(0, 2*i):
            print(" ", end="")
        for j in range(n, i, -1):
            print("*", end="")
        print()
    PrintLine(n)
    
# seventh pattern
# & if input is 8

#       *
#     ***
#   *****
# *******
# *******
#   *****
#     ***
#       *

def SeventhPatternE(n):
    i = 1
    rows = mt.ceil(n/2)
    while i <= rows:
        j = i
        while j < rows:
            # display space
            print(' ', end=' ')
            j += 1
        k = 1
        while k <= i:
            print('*', end=' ')
            k += 1
        print()
        i += 1
    i = rows+1
    while i >= 1:
        j = i
        while j <= rows:
            print(' ', end=' ')
            j += 1
        k = 1
        while k < i:
            print('*', end=' ')
            k += 1
        print('')
        i -= 1
    PrintLine(n)
    


# sevententh when odd

#       *
#     ***
#   *****
# *******
#   *****
#     ***
#       *

def SeventhPatternO(n):
    i = 1
    rows = mt.ceil(n/2)
    while i <= rows:
        j = i
        while j < rows:
            # display space
            print(' ', end=' ')
            j += 1
        k = 1
        while k <= i:
            print('*', end=' ')
            k += 1
        print()
        i += 1

    i = rows
    while i >= 1:
        j = i
        while j <= rows:
            print(' ', end=' ')
            j += 1
        k = 1
        while k < i:
            print('*', end=' ')
            k += 1
        print('')
        i -= 1
    PrintLine(n)

# Eighth Pattern 
# 12345
# 6789
# 012
# 34
# 5

def EightPattern(n):
    k = 1
    for i in range(n+1):
        j = 0
        while j < (n-i):
            k = k % 10
            print(f'{k}', end=" ")
            k += 1
            j += 1
        print()
    PrintLine(n)


# Ninth Pattern

#  1
#  234
# 56789
# 01234
#  567
#    8

def NinthPattern(n):
    l = 1
    for a1 in range(1, (n+1)//2 + 1):  # from row 1 to 5
        for a2 in range((n+1)//2 - a1):
            print(" ", end="")
        for a3 in range((a1*2)-1):
            l = l % 10
            print(l, end="")
            l += 1
        print()

    for a1 in range((n+1)//2 + 1, n + 1):  # from row 6 to 9
        for a2 in range(a1 - (n+1)//2):
            print(" ", end="")
        for a3 in range((n+1 - a1)*2 - 1):
            l = l % 10
            print(l, end="")
            l += 1
        print()
    PrintLine(n)

# tenth pattern 

# 0
# 10
# 010
# 1010

def TenthPattern(n):
    k = 0
    for i in range(0, n):

        # inner loop to handle number of columns
        # values changing acc. to outer loop
        for j in range(0, i+1):

            # printing 1 and 0 
            k = k % 2
            print(k, end="")
            k += 1
        # ending line after each row
        print("\r")
    PrintLine(n)

# driver function

# input the number of lines you need to print the pattern 
n = int(input("enter the number : "))
# first pattern 
FirstPattern(n)
# Second pattern 
SecondPattern(n)
# Third Pattern
ThirdPattern(n)
# Fourth Pattern
FourthPattern(n)
# Fifth Pattern 
if n % 2:
    FifthPatternO(n)
else:
    FifthPatternE(n)

# Sixth Pattern
if n % 2:
    SixthPatternO(n)
else:
    SixthPatternE(n)

# Seventh Pattern 
if n % 2:
    SeventhPatternO(n)
else:
    SeventhPatternE(n)

# Eight Pattern
EightPattern(n)

# Ninth Pattern
NinthPattern(n)

# Tenth Pattern
TenthPattern(n)
```

 Test Cases : 
```
# for n = 10 
# enter the number : 10
# * 
# * *
# * * *
# * * * *
# * * * * *
# * * * * * *
# * * * * * * *
# * * * * * * * *
# * * * * * * * * *
# * * * * * * * * * *

# ______________________
#          *
#         * *
#        * * *
#       * * * *
#      * * * * *
#     * * * * * *
#    * * * * * * *
#   * * * * * * * *
#  * * * * * * * * *
# * * * * * * * * * *

# ______________________
# * * * * * * * * * *
# * * * * * * * * *
# * * * * * * * *
# * * * * * * * 
# * * * * * *
# * * * * *
# * * * *
# * * *
# * *
# *


# ______________________
# **********
#   *********
#     ********
#       *******
#         ******
#           *****
#             ****
#               ***
#                 **
#                   *

# ______________________
# *
# * *
# * * *
# * * * *
# * * * * *
# * * * * *
# * * * *
# * * *
# * *
# *


# ____________

#         *
#       **
#     ***
#   ****
# *****
#   ****
#     ***
#       **
#         *

# ____________
#         *
#       * *
#     * * *
#   * * * *
# * * * * *
# * * * * *
#   * * * *
#     * * * 
#       * *
#         *


# ______________________
# 1 2 3 4 5 6 7 8 9 0
# 1 2 3 4 5 6 7 8 9
# 0 1 2 3 4 5 6 7
# 8 9 0 1 2 3 4
# 5 6 7 8 9 0
# 1 2 3 4 5
# 6 7 8 9
# 0 1 2
# 3 4
# 5


# ______________________
#     1
#    234
#   56789
#  0123456
# 789012345
#  678901234
#   5678901
#    23456
#     789
#      0

# ______________________
# 0
# 10
# 101
# 0101
# 01010
# 101010
# 1010101
# 01010101
# 010101010
# 1010101010

# ______________________





# 2 . n = 11 
# enter the number : 11
# * 
# * *
# * * *
# * * * *
# * * * * *
# * * * * * *
# * * * * * * *
# * * * * * * * *
# * * * * * * * * *
# * * * * * * * * * *
# * * * * * * * * * * *

# ________________________
#           *
#          * *
#         * * *
#        * * * *
#       * * * * *
#      * * * * * *
#     * * * * * * *
#    * * * * * * * *
#   * * * * * * * * *
#  * * * * * * * * * *
# * * * * * * * * * * *

# ________________________
# * * * * * * * * * * *
# * * * * * * * * * *
# * * * * * * * * *
# * * * * * * * *
# * * * * * * *
# * * * * * * 
# * * * * *
# * * * *
# * * *
# * *
# *


# ________________________
# ***********
#   **********
#     *********
#       ********
#         *******
#           ******
#             *****
#               ****
#                 ***
#                   **
#                     *

# ________________________
# *
# * *
# * * *
# * * * *
# * * * * *
# * * * * * *
# * * * * * 
# * * * *
# * * *
# * *
# *


# ______________

#           *
#         **
#       ***
#     ****
#   *****
# ******
#   *****
#     ****
#       ***
#         **
#           *

# ______________
#           *
#         * *
#       * * *
#     * * * *
#   * * * * *
# * * * * * *
#   * * * * *
#     * * * *
#       * * *
#         * *
#           *


# ________________________
# 1 2 3 4 5 6 7 8 9 0 1
# 2 3 4 5 6 7 8 9 0 1 
# 2 3 4 5 6 7 8 9 0
# 1 2 3 4 5 6 7 8
# 9 0 1 2 3 4 5
# 6 7 8 9 0 1
# 2 3 4 5 6
# 7 8 9 0
# 1 2 3
# 4 5
# 6


# ________________________
#      1
#     234
#    56789
#   0123456
#  789012345
# 67890123456
#  789012345
#   6789012
#    34567
#     890
#      1

# ________________________
# 0
# 10
# 101
# 0101
# 01010
# 101010
# 1010101
# 01010101
# 010101010
# 1010101010
# 10101010101

```


Question 16. Write a program which finds four digit perfect squares where the number represented by the first two digits and the number represented by the last two digits are also perfect squares.

```
# program to find the number which is perfect square and first and last two digit is also perfect square ... 

# driver code 

# importing math for ceil and floor 
import math as mt

# printing those numbers 
print("Four digit perfect Square number which has first two and lst two digit are also perfect square :\n");

# loop will cover all the four digit number 
for j in range(1000,10000) : 
    LastTwo = j%100             #Extracting last two digits
    FirstTwo = j//100           #Extracting first two digits

    #Checking whether the first two digits are perfect squares
    flag1=0   

    #Remember i is integer whereas sqrt() returns double 

    # As  as sqrt will be integer so floor and ceil of the number will be equal 

    if mt.ceil(mt.sqrt(FirstTwo)) == mt.floor(mt.sqrt(FirstTwo)) : 
        flag1=1 

    #Checking whether the last two digits are perfect squares
    flag2=0 

    if mt.ceil(mt.sqrt(LastTwo)) == mt.floor(mt.sqrt(LastTwo)) : 
        flag2=1 ;

    # Checking whether the number itself is a perfect square
    flag3=0 ;

    if mt.ceil(mt.sqrt(j)) == mt.floor(mt.sqrt(j)) : 
        flag3 = 1 ;

    if flag1==1 and flag2 ==1 and flag3==1 : 
        print(j,end=" "),
```

test cases : 
```
# only 1 case : 1600 1681 2500 3600 4900 6400 8100
```

Question 17. If a number 972 is entered through the keyboard, your program should print "Nine Seven Two". Write the program such that it does this for any positive integer.

```
# the program is used to find the wording of the number till 9 digit numbers can be easily extended to 20 digit number



# making array to deal with words is to make array indexing simple 
one = ["", "one ", "two ", "three ", "four ","five ", "six ", "seven ", "eight ","nine ", "ten ", "eleven ", "twelve ","thirteen ", "fourteen ", "fifteen ","sixteen ", "seventeen ", "eighteen ","nineteen "]

# strings at index 0 and 1 are not used,
# they is to make array indexing simple 
ten = ["", "", "twenty ", "thirty ", "forty ","fifty ", "sixty ", "seventy ", "eighty ","ninety "]

# n is 1- or 2-digit number


def numToWords(n, s):
    str = ""
    # if n is more than 19, divide it
    if (n > 19):
        str += ten[n // 10] + one[n % 10]
    else:
        str += one[n]
    # if n is non-zero
    if (n):
        str += s
    return str



# Function to print a given number in words
def convertToWords(n):
    # stores word representation of given
    # number n
    out = ""
    
    # handles digits at ten millions and
    # hundred millions places (if any)
    out += numToWords((n // 10000000),"crore ")

    # handles digits at hundred thousands
    # and one millions places (if any)
    out += numToWords(((n // 100000) % 100),"lakh ")

    # handles digits at thousands and tens
    # thousands places (if any)
    out += numToWords(((n // 1000) % 100),"thousand ")

    # handles digit at hundreds places (if any)
    out += numToWords(((n // 100) % 10),"hundred ")

    if (n > 100 and n % 100):
        out += "and "

    # handles digits at ones and tens
    # places (if any)
    out += numToWords((n % 100), "")

    return out

# Driver code


# long handles upto 9 digit no

# input 
n = int(input("enter the number : "))
if n<0 : print("number is negative")
if n == 0 : 
    print("Zero")
else : 
    # convert given number in words
    print(convertToWords(n))

```
test cases : 
```
# 1 . 12345 : twelve thousand three hundred and forty five 
# 2. 97456234 : nine crore seventy four lakh fifty six thousand two hundred and thirty four 
# 3 . 0 : zero 
# 4 . -5 : number is negative 
```

```
# program to print the number of digit in letter format 

# this function will print the word 

def Word(n)  : 
    if n == 0 : 
        print("zero", end=" "),
    if n == 1 :
        print("one", end=" "),
    if n == 2 :
        print("two", end=" "),
    if n == 3 :
        print("three", end=" "),
    if n == 4 :
        print("four", end=" "),
    if n == 5 : 
        print("five", end=" "),
    if n == 6 : 
        print("six", end=" "),
    if n == 7 : 
        print("seven", end=" "),
    if n == 8 :
        print("eight", end=" "),
    if n == 9 : 
        print("nine", end=" "),
        

# this is for reversing the numbers 
def Reverse(n1) : 
    res = 0
    while n1 > 0:
        res = (res*10) + (n1 % 10)
        n1 = int(n1/10)
    return res 


# driver code :  

# taking inputs : 
n = int(input("enter the number "))

if n>=0 : 
  # first reverse the number and then we will print the output
  res = Reverse(n) 

  # reversing will help to print the first number word first as they occur

  while res > 0 : 
      Word(res%10)
      res = res//10
```

test cases : 
```
# 1 . number : 972 , word = nine seven two 
# 2 . number : 11111 , word = one one one one one 

```

Question 18. If a number 972 is entered through the keyboard, your program should print "Nine hundred Seventy Two". Write the program such that it does this for any positive integer.

```
# the program is used to find the wording of the number till 9 digit numbers can be easily extended to 20 digit number



# making array to deal with words is to make array indexing simple 
one = ["", "one ", "two ", "three ", "four ","five ", "six ", "seven ", "eight ","nine ", "ten ", "eleven ", "twelve ","thirteen ", "fourteen ", "fifteen ","sixteen ", "seventeen ", "eighteen ","nineteen "]

# strings at index 0 and 1 are not used,
# they is to make array indexing simple 
ten = ["", "", "twenty ", "thirty ", "forty ","fifty ", "sixty ", "seventy ", "eighty ","ninety "]

# n is 1- or 2-digit number


def numToWords(n, s):
    str = ""
    # if n is more than 19, divide it
    if (n > 19):
        str += ten[n // 10] + one[n % 10]
    else:
        str += one[n]
    # if n is non-zero
    if (n):
        str += s
    return str



# Function to print a given number in words
def convertToWords(n):
    # stores word representation of given
    # number n
    out = ""
    
    # handles digits at ten millions and
    # hundred millions places (if any)
    out += numToWords((n // 10000000),"crore ")

    # handles digits at hundred thousands
    # and one millions places (if any)
    out += numToWords(((n // 100000) % 100),"lakh ")

    # handles digits at thousands and tens
    # thousands places (if any)
    out += numToWords(((n // 1000) % 100),"thousand ")

    # handles digit at hundreds places (if any)
    out += numToWords(((n // 100) % 10),"hundred ")

    if (n > 100 and n % 100):
        out += "and "

    # handles digits at ones and tens
    # places (if any)
    out += numToWords((n % 100), "")

    return out

# Driver code


# long handles upto 9 digit no

# input 
n = int(input("enter the number : "))
if n<0 : print("number is negative")
if n == 0 : 
    print("Zero")
else : 
    # convert given number in words
    print(convertToWords(n))

```
test cases : 
```
# 1 . 12345 : twelve thousand three hundred and forty five 
# 2. 97456234 : nine crore seventy four lakh fifty six thousand two hundred and thirty four 
# 3 . 0 : zero 
# 4 . -5 : number is negative 
```

19. Develop a program that receives the month and year from the keyboard as integers and prints the calendar in the following format. Note that according to the Gregorian calendar 01/01/1900 was Monday. With this as the base the calendar should be generated.


     September 2004
 Mon  Tue  Wed  Thu  Fri  Sat  Sun
            1    2    3    4     5
 6     7    8    9   10   11    12
13    14   15   16   17   18    19
20    21   22   23   24   25    26
27    28   29   30

```

#  program to output the month in calender format :


# Leap year is for finding whether the year is leap 

def LEAP(n):
    if n % 100 == 0:
        if n % 400 == 0:
            return True
    if n % 4 == 0:
        return True
    return False

# defining days array for corresponding months to find the number of days   
Days = [0, 31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]

# Driver Code 

# input of year and month 
year = int(input("Enter the year : "))
month = int(input("Enter the month : "))

# finding the difference of year which will help in finding the number of leap year and number of odd days 
diff = year - 1900
leaps = diff // 4

# if the given year is leap year then we will subtract one from total leaps as till now we have not finished that year , this help in finding the correct number of odd days , here we are finding odd days which help us to judge from which day the current month will start ... 
if LEAP(year):
    leaps -= 1

# as leaps year has 2 odd days 
oddDays = leaps*2

# and ordinal year has 1 odd day , 
oddDays += diff - leaps 

# now we are adding the days in the odd days which give us the total odd days 
for i in range(1, month):
    oddDays += Days[i]
if LEAP(year) and month > 2:
    oddDays += 1
# after getting total odd days we can find the starting day of the month which will be %7 of the total number of odd days
oddDays = oddDays % 7

# printing month and year 
if month == 1:
    print("\n\t\tJanuary")
elif month == 2:
    print("\n\t\tFebruary")
elif month == 3:
    print("\n\t\tMarch")
elif month == 4:
    print("\n\t\tApril")
elif month == 5:
    print("\n\t\tMay")
elif month == 6:
    print("\n\t\tJune")
elif month == 7:
    print("\n\t\tJuly")
elif month == 8:
    print("\n\t\tAugust")
elif month == 9:
    print("\n\t\tSeptember")
elif month == 10:
    print("\n\t\tOctober")
elif month == 11:
    print("\n\t\tNovember")
elif month == 12:
    print("\n\t\tDecember")
print(f'\t {year}\n\n')

# printing the calender format 
print("\n\nMon   Tue   Wed   Thu   Fri   Sat   Sun\n\n")

# giving blank space before the actual day of the month 
for i in range(oddDays):
    print("     ", end=""),

# now for leap year in month of feb has 29 days which will in making the calender perfect 
if LEAP(year) and month == 2:
    day = 29
else:
    day = Days[month]
    

# now printing the calender format 
for i in range(1, day+1):
    if (i+oddDays) % 7 == 1:
        print("\n", end=""),
    print("{blc:5d}".format(blc=i), end="")
```

test cases : 
```
# 1 .  year 1901 , month 1 , 
# output : 

            # January  1901 
# Mon   Tue   Wed   Thu   Fri   Sat   Sun


#          1    2    3    4    5    6
#     7    8    9   10   11   12   13
#    14   15   16   17   18   19   20
#    21   22   23   24   25   26   27
#    28   29   30   31



#2 .  year 2004 , month 9 

        
        #September 2004 
# Mon   Tue   Wed   Thu   Fri   Sat   Sun


#              1    2    3    4    5
#    6    7    8    9   10   11   12
#   13   14   15   16   17   18   19
#   20   21   22   23   24   25   26
#   27   28   29   30

```

QUESTION 20. Write the function digits(n) that returns how many digits the number has. For example: 25 has 2 digits and 144 has 3 digits.
 

```
#  this program is used to find the number of digit in the number 

# Function to find the number of digits in the number
def Count_Digit(n) : 
    count = 0 
    # here this while loops divides and reduce one digit every time it is greater than 0
    while n>0: 
        n = n//10
        count += 1
    return count


#  driver code 

# input number 
n  = int(input("enter the number "))
print(f'the number of digits is : {Count_Digit(n)}')
```
test cases :
```
# 1 . n = 10 , digits = 2 
# 1 . n = 102 , digits = 3 
# 1 . n = 10234 , digits = 5 

```

21. Write a function to print out a multiplication table (where each number is the result of multiplying the first number of its row by the number at the top of its column). Demonstrate by calling multiplication_table(1, 3) will print out:
1 2 3
2 4 6
3 6 9

```
# program to find the multiplication table 

def MultiplicationTable(a,b): 
    for i in range(a): 
        for j in range(b):
            # here we know that the index are multiplied which show the value at the multiplication table
            print((i+1)*(j+1), end=' '),
        print()

#driver function

# take input for the multiplication table 
a = int(input("enter the value of a "))
b = int(input("enter the value of b "))
MultiplicationTable(a,b)
```
 test cases : 
```
# 1 . a = 5 , b = 10 ,
# Multiplication table is : 
# 1 2 3 4 5 6 7 8 9 10 
# 2 4 6 8 10 12 14 16 18 20
# 3 6 9 12 15 18 21 24 27 30
# 4 8 12 16 20 24 28 32 36 40
# 5 10 15 20 25 30 35 40 45 50

# 2 . a = 15 , b = 5 
# Multiplication table is : 
# 1 2 3 4 5     
# 2 4 6 8 10    
# 3 6 9 12 15   
# 4 8 12 16 20  
# 5 10 15 20 25 
# 6 12 18 24 30 
# 7 14 21 28 35
# 8 16 24 32 40
# 9 18 27 36 45
# 10 20 30 40 50
# 11 22 33 44 55
# 12 24 36 48 60
# 13 26 39 52 65
# 14 28 42 56 70
# 15 30 45 60 75
```

QUESTION 22. Write a  counter function which counts down from start to stop when start is bigger than stop, and counts up from start to stop otherwise. I.e. print(counter(1, 10)) # Should be "Counting up: 1,2,3,4,5,6,7,8,9,10"

```
# here in this program we step up start is less than stop otherwise we step down 

# function to do the step up or step down in counting and print the step count 
def counter(start,stop) : 
    # check if start is less than stop if yes then step up 
    if start<stop : 
        for i in range(start,stop) : 
            print(i,end = ","),
        print(stop)
    # else if start greater than step down 
    elif start>stop : 
        for i in range(start,stop,-1) : 
            print(i,end = ","),
        print(stop)
    # other the start and stop are at same place then print only start 
    else : 
        print(start)

# driver program for inputs and outputs
# input start 
Start = int(input("Enter the Start : "))
# input stop
Stop = int(input("Enter the Stop : "))
# calling the function 
counter(Start,Stop)
```
test cases : 
```
# 1 . start : 1 , stop : 5 , output : 1,2,3,4,5
# 2 . start : 10 , stop : 4 , output : 10,9,8,7,6,5,4
# 2 . start : 11 , stop : 11 , output : 11
```

QUESTION 23. Write the print_prime_factors function which will print all the prime factors of a number. A prime factor is a number that is prime and divides another without a remainder.

```
# for factorization of a number in O(log(n)) time complexity  i am using sieve Factorization for the implementation it is fastest to find the factorization,the basic idea in this is we store the smallest number which divides the particular number at there index and then we divide the number with that smallest number and we get the index of the number which is a multiple of that number and it goes on till we get 1 ... 


#import math for sqrt and ceil function 
import math as mt 
# MAXN is for the size of the array which stores the factors of the numbers 
MAXN = 100001
# factors is the array which will store the factors of the numbers 
factors = [0 for i in range(MAXN)]

# this function will be used to find the factors and store them in the factors array 
def factorise() : 
    factors[1] = 1
    # this following loop is used to store the number itself as every number divide itself 
    for i in range(2,MAXN) : 
        factors[i] = i
    # this following loop is use to marks the even numbers in the array 
    for i in range(4,MAXN,2): 
        factors[i] = 2
    # this loop is to spot the prime factors 
    for i in range(3,mt.ceil(mt.sqrt(MAXN))) : 
        if factors[i] == i : 
            for j in range(i*i , MAXN,i): 
                if factors[j] == j : 
                    factors[j] = i 

# this function is used to fetch the factors of the numbers from array 
def getFactors(n) : 
    # creating an list to keep track of the factors of the numbers 
    get = list()
    while n!=1 : 
        # adding the factors of the numbers to the list
        get.append(factors[n])
        # divding the number with factor to get the next factor of the remaining number
        n = n // factors[n] 
    return get # returning the list 

# function to print the prime factors 
def print_prime_factors(n) : 
    # calling the function to get the prime factors of the numbers  in the list fac 
    fac = getFactors(n)
    for i in range(len(fac)): 
        print(fac[i],end = " ")

# calling the factorise function to get the smallest prime factor of every number. 
factorise()

# driver code for input and calling the function
n = int(input("enter the number whose input "))
print_prime_factors(n)

# constraints 
# 1 . n<=1e5 we can find more for that we increase MAXN and increase upto 1e7 or 1e8 according to the system . we can also find for greater number but for that we can't have array greater than 1e7 size . 
# if n>1e9 we can use loop and direct print the result instead of storing the result but that will increase some time , here we are getting the result in O(1) constant time as it stored we just need index but  in that case it will take O(log(n)) time to fetch the result ... that the reason i choose this one ... 
```
some test cases :
```
# 1 . for 1000 : 2 2 2 5 5 5        
# 2 . for 12345 : 3 5 823 
# 3 . for 98765 : 5 19753
# 4 . for 11111 : 41 271
# 5. for 512 : 2 2 2 2 2 2 2 2 2
```

QUESTION 24. The longest_word function is used to compare 3 words. It should return the word with the most number of characters (and the first in the list when they have the same length).

```

# here i am trying to print the string with most number of  characters it does not depend on the length of the string , as a string with "aaaa" has only  1 character  and "abc" has three character , i have implemented in such a way that the word "abc" is longer than "aaaa" .  most character is the longest word in my operation , as asked in the question  

# here we are declaring three array with 0 initial value  which stores 26 letter index for each word in this way we can figure out and increase the value of the array at the letter occur in the word  index i.e if 'a' occurred the arr[0] becomes 1 and so on  
w1 = [0 for i in range(27)]
w2 = [0 for i in range(27)]
w3 = [0 for i in range(27)]

# this longest word function find the longest words in term of most number of characters in the sentences (here i am assuming that most number of character means different character)
def longest_word(word1, word2, word3):
    
    # here lower case the words to make it proper for finding index of the array otherwise it can be large 'A' - 'a' which will be negative so creates trouble  
    word11 = word1.lower()
    word21 = word2.lower()
    word31 = word3.lower()
    # marking the different words present in the words 
    for i in range(len(word11)):
        if (ord(word11[i])- ord('a')) < 26  and (ord(word11[i])- ord('a')) >= 0 :
            w1[ord(word11[i]) - ord('a')] += 1
    for i in range(len(word21)):
        if (ord(word21[i])- ord('a')) < 26  and (ord(word21[i])- ord('a')) >= 0 :
            w2[ord(word21[i]) - ord('a')] += 1
    for i in range(len(word31)):
        if (ord(word11[i])- ord('a')) < 26  and (ord(word11[i])- ord('a')) >= 0 :
            w3[ord(word31[i]) - ord('a')] += 1
    # now finding the length of the words in term of total number of different words in the sentence 
    len1 = 0 
    len2 = 0
    len3 = 0
    for i in range(27):
        if w1[i]:
            len1 += 1
    for i in range(27):
        if w2[i]:
            len2 += 1
    for i in range(27):
        if w3[i]:
            len3 += 1
    # now comparing the length and if length of the words are equal then first words will be the longest words
    if len1>= len2 and len1 >= len3:
        word = word1
    elif len2 >= len1 and len2 >= len3:
        word = word2
    else:
        word = word3
    # now printing the longest word  
    print(word)

# drivers code 
# taking three inputs as strings
word1 = input("enter the word 1 ")
word2 = input("enter the word 2 ")
word3 = input("enter the word 3 ")
# calling the function 
longest_word(word1, word2, word3)
```
 some test cases 
 ```
#  1 . longest_word("Ashish", "kumar", "IIITK")  ans : kumar with 5 most number of different character 
# 2 . longest_word("AAAA", "AAAAA", "AAAAAA") ans : "AAAA" as all have only one character "A" so first will be the ans when length of different character is same 
```
Other Way
```
# advantage of the code is that : it will read only characters as  length of the words otherwise user can give input numbers and white spaces which will not be considered as characters 

# disadvantage of the code is that it will consider 'A' and 'a' as same though it is not same but it will consider that ... 

# if we define longer words as word with longer length 
# then below good is the best for that 
# this function only compare the length of the word 
def longestWord(word1, word2, word3):
    if len(word1) >= len(word2) and len(word1) >= len(word3):
        word = word1
    elif len(word2) >= len(word1) and len(word2) >= len(word3):
        word = word2
    else:
        word = word3
    print(word)

# taking three inputs as strings
word1 = input("enter the word 1 ")
word2 = input("enter the word 2 ")
word3 = input("enter the word 3 ")
# calling the function 
longestWord(word1, word2, word3)
```
some test cases 
```
#  1 . longest_word("Ashish", "kumar", "IIITK")  ans : Ashish with length 6 and number of character : 6  
# 2 . longest_word("AAAA", "AAAAA", "AAAAAA") ans : "AAAAAA" as it has length 6 and number of character : 6 
```



## Python Worksheet 3


Question 1 : Write a program to show bits of an integer


Answer 1 : 
```
# This is the program to find the Binary form of the given number using bit manipulation 

# this function is used to find the binary form of the given number
def BinaryForm(n) : 
    # initializing a list for storing the each bit 
    list1 = []
    # to find the last 16 bits of the number
    for i in range(16):
        # finding whether the ith bit is set or not 
        if (n &(1<<i)) == 0 :
            list1.append(0)
        else :
            list1.append(1)
    # then reversing the list as it store all the bits in their reverse form 
    list1.reverse()
    print(list1)


# driver code 
# taking input 
n = int(input("enter the number : "))
# calling the function to find the binary form of the given number
BinaryForm(n)
```

test cases
```
# 1. n = 2  output = 0000000000000010
# 2. n = 12345 output = 0011000000111001
# 3. n = 123456 output = 1110001001000000
```




Question 2.) The information about colors is to be stored in bits of a variable called color. The bit numbers 0 to 6, each represents 7 colors of a rainbow, i.e. bit 0 represents violet, 1 represents indigo, and so on as given below. Write a program that asks the user to enter a number and based on this number it reports which colors in the rainbow does the number represents.
Red     Orange     Yellow      Green     Blue    Indigo	  Violet



Answer 2: 
```
# in this we have to find the name of the colors from the color list which corresponds to its set bit of the given number in its binary from

# the color list  
colors = ["Red","Orange","Yellow","Green","Blue","Indigo","Violet"]

# list to store the set and unset bits
list1 = []

# taking user input 
n = int(input("enter the number"))

# code to find the name of the color from the list
# as it will search only till the length of the list in the list  
for i in range(len(colors)):
    # it is checking the ith bit is set or not
    if (n &(1<<i)) == 0 :
        list1.append(0)
    else :
        list1.append(1)

# as list has to be reverse because the bit are append in the list so to make it use in proper order , reverse it .  
list1.reverse()

# display of the colors
for i in range(len(colors)): 
    if list1[i] : 
        print(colors[i],end=' ')
```
test cases : 
```
# 1. n= 23 colors = Yellow Blue Indigo Violet
# 2.  n = 127 colors = Red Orange Yellow Green Blue Indigo Violet
# 3. n = 12345  colors = Orange Yellow Green Violet

# the reason for larger number to show less colors because other set bits of the number is not in range of this seven .
```



Question 3.) In an inter-college competition, various sports and games are played between different colleges like cricket, basketball, football, hockey, lawn tennis, table tennis, carom and chess. The information regarding the games won by a particular college is stored in bit numbers 0, 1, 2, 3, 4, 5, 6, 7 respectively of an integer variable called game. The college that wins in 5 or more than 5 games is awarded the Champion of Champions trophy. If a number is entered through the keyboard, then write a program to find out whether the college won the Champion of the Champions trophy or not.


Answer 3 : 
```
# in this we have to find the number of games a team won from the  list which corresponds to its set bit of the given number in its binary from and according to that champions of champions is to find for the given condition .           

# list of games . 
sports = ["Cricket","BasketBall","Football","Hockey","Lawn Tennis","Table Tennis","Carrom","Chess"]

# list to store the set and unset bits
list1 = []

# taking user input
n = int(input("enter the number"))

for i in range(len(sports)):
    if (n &(1<<i)) == 0 :
        list1.append(0)
    else :
        list1.append(1)

count = 0

# counting the number of games won
for i in range(8):
    if list1[i]:
        count+=1

# checking the condition for champion fo champions 
if count>=5 : 
    print("Congratulation your team won Champions OF Champions Trophy")
else : 
    print("Sorry Better Luck Next Time for the Trophy ")

```



Question 4.)The time field in the directory entry is 2 bytes long. The distribution of different bits which account for hours, minutes, and seconds is given below. Write a program that would receive the two-byte time entry in form of a number and print the hours, minutes, and seconds.
 H H H H H M M M M M M S S S S S


Answer 4:
```
# find time in this format HHHHHMMMMMMSSSSS 
# I am taking input as number and taking the 16 bit binary form and for first five finding hour and for the next six finding minutes and for the last 5 finding seconds.

# taking input
n = int(input("enter the number : "))

# list to store the bits  
list1 = []
# for 16 bits 
for i in range(16):
    if (n &(1<<i)) == 0 :
        list1.append(0)
    else :
        list1.append(1)
list1.reverse()
# finding hours , minutes and seconds 
hr = 0
mn = 0
sec = 0
# first five for hours and converting set bits in numbers 
for i in range(4,0,-1):
    if list1[i]:
        hr+= 2**i

#then 6 for minutes  
for i in range(10,5,-1):
    if list1[i]:
        mn += 2**(i-5)

# then last five for seconds 
for i in range(15,11,-1):
    if list1[i]:
        sec+= 2**(i-11)
print(f'the time is {hr} hours {mn} minutes {sec} seconds ')
```

test cases for
```
# 1. n = 12345  output : 12 hours 32 minutes 18 seconds
# 2. n = 446 output : 0 hours 44 minutes 14 seconds 
```



Question 5.) Write a program to encrypt/decrypt using a bitwise operator.   (A,K = En    En,K = A)

Answer 5 : 
```
# code for encrypt and decrypt the message using bitwise xor 

num = int(input("enter the number you want to encrypt : "))

# for using xor property 
# taking a default number of characters

# let bydefault as default number 
bydefault = 9999

print(f'the encrpt is {num^bydefault}')
```
test cases : 
```
# 1 . number = 123456  encrypt = 11607  for default = 9999 
# 2 . number = 999999 encrypt = 1008944
```




Question 6) Write a program to check if Kth bit of N is set or not. A bit is called set if it is 1. Position of set bit '1' should be indexed starting with 0 from LSB side in the binary representation of the number.


Answer 6 : 
```
# program to check the kth set bit 

# driver code          
n = int(input("enter the number : "))
k = int(input("enter the bit you want check:"))
# cheking by shifting 1 to k left bit and if there and is 1 then it set and not then not a set bit set
if (n & 1<<k) : 
    print("Yes it is set ")
else:
    print("no it is not set")
```    

test cases : 
```
# 1. n = 1234 , k = 5 , output = not set 
# 2. n = 2 , k = 1 , output = set bit (as it will 10 as 0 from lsb given that means we can check for k = 0 )

# 3 . n = 1 , k = 0 , output = set bit  
```




Question 7.) Write a program to Swap two numbers without using an intermediate variable using a bitwise operator. 
Answer 7 : 
```
# swaping the number without using the third variable 
a = int(input("enter the first number : "))
b = int(input("enter the second number : "))
# using xor property to avoid the third variable
a = a^b;
b = a^b;
a = a^b;
print(f'value of a is {a} and b is {b}')
```
test cases : 
```
# 1. a = 3 , b = 4 , output = value of a is 4 and b is 3
# 2. a = 5 , b = 10 , output = value of a is 10 and b is 5

```



Question 8.) Write a program to swap the two nibbles in it and find the resulting number. For example, input number is 100 then Output: 70. 100 in binary is 01100100, two nibbles are (0110) and (0100) If we swap the two nibbles, we get 01000110 which is 70 in decimal. 

Answer 8 : 
```
# swapping the two nibbles in the binary representation of a given number and then converting it into the new number 

# function to swap the nibble 
def nibbles(x):
    # as bin is use to convert it into binary representation [2:] will slice it from 2 to the end as binary numbers are represented by '0b11001010' so this will get rid off the '0b' from the starting. 
    bin_num=bin(x)[2:].zfill(8)
    print("Enter binary number: ",end='')
    print(bin_num)
    # swapping the nibbles as it nibble contains four bits  
    new_num=bin_num[4:8]+bin_num[0:4]
    print("Swapped binary number: ", end='')
    print(new_num)
    # converting number to decimal representation
    a=int(new_num,2)
    print("New Decimal number formed by swapping: ", end='')
    print(a)
    
# driver code  
# taking input 
n = int(input("enter the number : "))
nibbles(n)
```
 test cases :
```
# 1. n = 10 
# output : Enter binary number: 00001010
# Swapped binary number: 10100000
# New Decimal number formed by swapping: 160

# 2. n = 12345
# output : Enter binary number: 11000000111001
# Swapped binary number: 00001100
# New Decimal number formed by swapping: 12

# 3. n =  99999999
# output: Enter binary number: 101111101011110000011111111
# Swapped binary number: 11101011
# New Decimal number formed by swapping: 235
```


Question 9.) Write a program to find the total number of bits needed to be flipped to convert one integer to another.


Answer 9 : 
```
# program to find the number of bit require to change while converting one number into another

# function to count bits  
def change(a,b):
    count = 0
    # as we know using xor can find the position where the bits are different as xor for two different bit is 1 so we can use that in here .
    a = a^b;
    # for ex if a = 1010 and b = 1101 the a^b is 0111 as last three bits are different so all will be one now we have to calculate the number of set bits in a^b
    
    # using while a is not zero 
    # as a & (a-1) as now a^b = 0111 now if we and (0111 & 0110)= 0110  we get rid of one 1 from the binary representation and we increse count , similarly doing till a is 0
    while a :
        a = a & (a-1)
        count+=1
    return count

# driver code 
a = int(input("enter the first number : "))
b = int(input("enter the number you want to convert : "))
print(f'number of bits changes while changing  {a} to {b} is {change(a,b)}')
```
test cases :
```
# 1.  a = 10 , b = 13 , output = 3
# 2. a = 100, b = 111 , output = 3
# 3. a = 1000 , b = 1111 , output = 10
```




Question 10.)Write a program to Round up to the next highest power of 2
Answer 10 : 
```
# program to find the next power to two   

# function to find the next power
def findNextPowerOf2(n):
	n = n - 1
	# as n can be itself power of two 

	# doing till only one bit is left
	while n & n - 1:
		n = n & n - 1   	# unset rightmost bit 
	# return next power of 2
	return n << 1

# driver code 
n = int(input("enter the number whose next power of 2 is to be found : "))
print(f'the next power of 2 for {n} is {findNextPowerOf2(n)}')
```
test cases 
```
# 1. n = 16 , output = 16 
# 2. n = 20 , output = 32
# 3. n = 123456789 , output = 134217728
```




Question 11.)Write a program to swap all odd bits with even bits. For example, if the given number is 23 (00010111), it should be converted to 43(00101011). Here, every even position bit is swapped with an adjacent bit on the right side(even position bits are highlighted in the binary representation of 23), and every odd position bit is swapped with an adjacent on the left side.


Answer 11: 
```
# program to swap the odd bits with even bits

# taking input
num = int(input("enter the number : "))
# taking even and odd number as zero
even = 0
odd = 0

# as it will increment by two and swapping the odd and even bits of that particular pair as even number will 1 less than odd position if we take as 0 from LSB , with that we can find the even and odd bits and if we substract if from the number and again shift by one in alternate direction will give the number on addition of odd and even
for i in range(1, 32, 2):
    even = num & (1 << (i-1))
    odd = num & (1 << i)
    num = num-even-odd
    even = even << 1
    odd = odd >> 1
    num = num+even+odd

# printing the new number
print(num)
```
test cases :
```
# 1. n = 12345 , output : 12342
# 2. n = 99999 , output : 149871
# 3. n = 98765, output :  148174
```



Question 12.)Write a program to find the 1's complement of the given number. The ones' complement of a binary number is defined as the value obtained by inverting all the bits in the binary representation of the number (swapping 0s for 1s and vice versa).


Answer 12: 
```
# to find the one's complement of the we use tilder as it changes the bits
import math

n = int(input("enter the number : "))
print(f'the number is {~n} ')

# output :
# 1. n = 10 , output = -11 (as the msb for 10 is 0 , so when it will be negative .)

# one interesting fact is that we can see the one's complement of a number is just the negative of increment of the number
# 2. n = 1111 , output : -1112
# 3. n = 1112, output : -1113


#ANOTHER WAY OF DOING THE QUESTION IS : 
# if we just want to find the one's complement of the number in its binary form (not upto 32 bits only upto till its binary representation for ex 1010 will be 101) like that then

# function to find the one's complement
# Finding n as number of bits in the given integer and then finding the 2^(n-1) xor with original number will give the result

def onesComplement(num):
    number_of_bits = (int)(math.floor(math.log(num) / math.log(2))) + 1
    return ((1 << number_of_bits) - 1) ^ num


# Driver code
num = int(input("enter the number : "))
print(onesComplement(num))

```
test cases :
```
# 1. n = 10 (1010) , output = 5 (0101)
# 2. n = 12345 , output = 4038
# 3. n = 99999. output = 31072
# 4. n = 2 , output = 1 
```



Question 13.)Write a program to count the set-bits and non-set-bits of an integer N.

Answer 13:
```
# program to find the set bits and non set bits
# finding set bits and suntracting from total bits


# function to find the total number of bits
def countBits(n):
    count = 0
    # shifting one by one until it is not zero
    while (n):
        count += 1
        n >>= 1
    return count

# finding number of set bits


def countSetBits(n):
    count = 0
    while (n):
        n = n & (n-1)
        count += 1
    return count


# drivers code
n = int(input("enter the number : "))
print(
    f' number of set bits are {countSetBits(n)} and number of unset bits are {countBits(n)-countSetBits(n)}')
```
test case :
```
# 1. n = 101   output : set bit = 4 and non set bits = 3
# 2. n = 12345 output : set bits = 6 and non set bits = 8
# 3. n = 98789 output : set bits = 8 and non set bits = 9
```



Question 14.)Write a program to check if a number is a power of 8 or not.

Answer 14:
```
# program to find whether the number is power of 8 or not

# function to check for power of 8  as if it power of 8 then it set bits must be at position which are multiple of 3 if we take lsb at 0 and then 2  from the first one and only set bit should at there in the entire binary representation


def Powerof8(n):
    # starting from 0 lsb checking for 32 bits 
    i = 0
    l = 1
    while (i <= 31):
        l <<= i
        if (l == n):
            return True
        i += 3
        l = 1
    return False

# driver code 
n = int(input("enter the number : "))
print(f' the number {n} is {Powerof8(n)} about the power of 8 ')
```
test cases : 
```
# n = 1 , output = yes 
# n = 8 , output = yes
# n = 16, output = no
# n = 64 , output = yes 
```

Question 15)Write a program to determine whether a number is odd or even using bitwise operators.

Answer 15: 
```

# function to find whether the number is even or odd.
def oddEven(n):
    if(n & 1 == 0):
        print(f'the number {n} is even')
    else:
        print(f'the number {n} is odd ')


# driver code
n = int(input("enter the number :"))
oddEven(n)
```
test cases :
```
# n = 1 , output = odd
# n = 2 , output = even
# n = 10 , output = even
# n = 1111 , output = odd
```

Question 16.)The Bit Game: Two players, Player 1 and Player 2, are given an integer N to play a game. The rules of the game are as follows :
a.)In one turn, a player can swap any 2 bits of N in its binary representation to make a new N.
b.)In one turn, a player has to make a number strictly less than N.
c.)Player 1 always takes the first turn.
d.)If a player cannot make a move, he loses.

Answer 16:
```
# program to find which player , as two player get chance to swap the number and find the smaller number than the previous if player cannot then it will lose

# function to find which player wins
# using the basic idea of dividing the number by two and will give the smaller number and it will change two bits following the condition of the game , and using the xor property on k and x , and incrementing the x when it is divisible by two will give the condition for k greater than 1 .
def bitGame(n):
    x = 0
    k = 0
    while n>0:
        if n%2 and x>0 :
            k = k^x
        if n%2 == 0:
            x+=1 
        n = n/2
    if k>0 :
        return 1
    else:
        return 2
n = int(input("enter the number :  "))
print(f'player {bitGame(n)} wins')
```
test cases : 
```
# 1. n = 8 , output :  player 1 wins
# 2. n = 1111 , output : player 2 wins
# 3. n = 9999, output : player 2 wins
```


Question 17.)Given two integers numbers N and K, Write a program to find f(f(..........f(N))) K times, where f(x) = x XOR (x%10). N = 66 and K= 3 So output will be 74.

Answer 17 : 
```
# program to find the functional value of f(....f(k)) where f(k) = x^(x%10)
# as if x%10 == 0 and xor of any number with zero gives the number itself otherwise finding it till k times

# function
def fun(n, k):
    for i in range(k):
        if(n % 10 == 0):
            return n
        n = n ^ (n % 10)
    return n


# driver code
n = int(input("enter the number : "))
k = int(input("enter the value of k : "))
print(f'the value of the operation is {fun(n,k)}')
```
 test cases :
```
# 1. n = 110 , k = 10 , output = 110 ,
# 2. n = 66 , k = 3 , output = 74
# 3. n = 9999 , k = 9999 , output = 9990 ,
```



Question 18.)Write a program to check if the binary representation of a number is palindrome or not.

Answer 18.)
```
#program to check whether binary representation of a number is palindrome


import sys
# function to check whether the kth bit is set or not 
def isKthBitSet(x, k):
	if ((x & (1 << (k - 1))) !=0):
		return True
	else:
		return False

#function  to check the palindrome
# checking using two pointer technique as moving from left and right and checking whether the corresponding bit are same or not , if yes then they move closer towards each other otherwise not palindrome 

def isPalindrome(num):
	left_bit = 1
	right_bit = 2 * 8 
	while (left_bit < right_bit):
		if (isKthBitSet(num, left_bit) != isKthBitSet(num, right_bit)):
			return False
		left_bit += 1
		right_bit -= 1
	return True
# driver code 
n = int(input("enter the number : "))
print(f'the number {n} is {isPalindrome(n)} about the plaidrom of its bits representation ')

```
test cases 
```
# 1. n = 1002 , output : not palindrome
# 2. n = 0 , output : yes palindrome
```

 ## Python WorkSheet 4 
Question 1 : Create two new classes for each real-world object that you observed. Use docstring to document the class well. Use __str__ to print a meaningful object description.


Ans 1: 
```
class HumanBeing:
    ''' Here The Class HumanBeing Asks For the Data Like Name and Age and return the format of their data.
    It has __init__ function which act initialise data to the class object and __str__ format about the 
    data in what way it is being stored '''
    
    # __init__ method to initialise the variables name and age . and we know that we can use anything in
    # place of self so i am using WhatIsYour
    def __init__(WhatIsYour,name,age):
        WhatIsYour.name = name
        WhatIsYour.age = age
    
    # here __str__ method gives the format of the variables and their description  
    def __str__(Your):
        return f'Your Name : {Your.name} and Your Age : {Your.age}'
    
    # added one method AddTitle to add title to the name of the Person
    def AddTitle(YourTitle,title):
        YourTitle.name = YourTitle.name+" "+title

# driver code 
# main method 
def main():
    Person1 = HumanBeing("Ashish",19)
    Person1.AddTitle("Kumar")
    print(f'{HumanBeing.__doc__}')
    print(f'{Person1.__str__()}')
    print(f'{Person1}')

#main() is called    
if __name__=="__main__" :
    main()


# output : 
#    
#  Here The Class HumanBeing Asks For the Data Like Name and Age and return the format of their data.
#     It has __init__ function which act initialise data to the class object and __str__ format about the 
#     data in what way it is being stored 
# Your Name : Ashish Kumar and Your Age : 19
# Your Name : Ashish Kumar and Your Age : 19
```


Question 2: 
Create a python class that illustrates a famous quote by George Bernard Shaw, using objects to represent people. “If you have an apple and I have an apple and we exchange these apples then you and I will still each have one apple. But if you have an idea and I have an idea and we exchange these ideas, then each of us will have two ideas.” (i.e. class Person with attributes apples, ideas, and methods exchange_apples(), exchange_ideas().) Use docstring to document the class well. Use __str__ to print a meaningful object description.


Ans : 
```
class Quotes:
    ''' This Class illustrate a very famous quote by George Bernard Shaw '''
    ''' initializing the number of apples and ideas each person has '''
    
    # init function to initialise variables 
    def __init__(self, apples,ideas):
        self.apples = apples
        self.ideas = ideas
    
    ''' when we exchange apples''' 
    def exchange_apples(self):
        print(f' if we exchange our {self.apples} apples with each other then we both will still have {self.apples} apples ')
    
    ''' when ideas are exchanged '''
    def exchange_ideas(self):
        print(f'if we both have {self.ideas} different idea then after sharing we are going to have {2*self.ideas} ideas ')
    
    ''' format of the class '''
    def __str__(self):
        return f'What we learn is exchanging {self.ideas} ideas will really help in growth but exchanging {self.apples} will not change the situation '

#main() is called
def main() :
    Quotes1 = Quotes(5,5)
    print(Quotes.__doc__)
    Quotes1.exchange_apples()
    Quotes1.exchange_ideas()
    print(Quotes1)
    
if __name__=="__main__":
    main()
    
    
#  output : 

# This Class illustrate a very famous quote by George Bernard Shaw 
# if we exchange our 5 apples with each other then we both will still have 5 apples 
# if we both have 5 different idea then after sharing we are going to have 10 ideas 
# What we learn is exchanging 5 ideas will really help in growth but exchanging 5 will not change the situation
```


Question 3 :
Create a Time class and initialize it with hours and minutes.
1. Make a method addTime which should take two time object and add them. E.g.- (2 hour and 50 min)+(1 hr and 20 min) is (4 hr and 10 min)
2. Make a method displayTime which should print the time.
3. Make a method DisplayMinute which should display the total minutes in the Time. E.g.- (1 hr 2 min) should display 62 minute.


Ans : 
```

class Time :
    ''' this class is for adding two class object's time and presenting the time in minutes only '''
    
    # init function is for initialise the hour and minutes 
    def __init__(self,hrs,mins):
        self.hrs = hrs
        self.mins = mins
    
    # add time for two objects
    def addTime(self,ob1,ob2):
        self.mins = (ob1.mins + ob2.mins)%60
        self.hrs = (ob2.hrs+ob1.hrs) + (ob1.mins+ob2.mins)//60
    
    # display the time 
    def displayTime(self):
        print(f'time is {self.hrs} hours and {self.mins} minutes')
    
    # display in minutes 
    def DisplayMinutes(self):
        print(f'time in minutes is : {self.hrs*60 + self.mins} minutes')
        
    def __str__(self):
        return f'time is {self.hrs} hours and {self.mins} minutes '

# driver code 
def main():
    hours1 = int(input("enter the hours : "))
    minutes1 = int(input("enter the minutes : "))
    time1 = Time(hours1,minutes1)
    time1.displayTime()
    time1.DisplayMinutes()
    hours2 = int(input("enter the hours : "))
    minutes2 = int(input("enter the minutes : "))
    time2 = Time(hours2,minutes2)
    time2.displayTime()
    time2.DisplayMinutes()
    print(f'Now adding the {time1} and {time2}')
    time1.addTime(time1,time2)
    time1.displayTime()
    time1.DisplayMinutes()

if __name__ == "__main__":
    main()
    

# output : 
# enter the hours: 12
# enter the minutes: 34
# time is 12 hours and 34 minutes
# time in minutes is : 754 minutes
# enter the hours:  45
# enter the minutes: 6
# time is 45 hours and 6 minutes
# time in minutes is : 2706 minutes

# Now adding the time is 12 hours and 34 minutes and time is 45 hours and 6 minutes
# time is 57 hours and 40 minutes
# time in minutes is : 3460 minutes
```



Question 4: 
The City class has the following attributes: name, country (where the city is located), elevation (measured in meters), and population (approximate, according to recent statistics). Write max_elevation_city function to return the name of the city and its country (separated by a comma), when comparing the 3 defined instances for a specified minimal population. Use docstring to document the class well. Use __str__ to print a meaningful object description. 

Ans : 
```
class City : 
    ''' this City class has different attribute for a city like city Name, county of the city , elevation 
    from sea level and the population of that city  and we are using a max_elevation_city function which takes a minimum_population by user checks whether that kind of city is available 
    with minimum that much populations and have maximum elevation'''
    
    # init function 
    def __init__(self,name,country,elevation,population):
        self.name = name
        self.country = country
        self.elevation = elevation
        self.population = population
    
    # maximim elevation function checks for maximum elevation with at least minimum population in it  
    def max_elevation_city(self,min_population, city1 , city2 , city3 ):
        return_city = city1
        if city1.population >= min_population:
            return_city = city1
        if city2.population >= min_population and city2.elevation > return_city.elevation:
            return_city = city2
        if city3.population >= min_population and city3.elevation > return_city.elevation:
            return_city = city3
        if return_city.name:
            return f"{return_city.name}, {return_city.country}" 
        else:
            return ""
        
    def __str__(self):
        return f'{self.name} city of {self.country} is elevated {self.elevation}m from sea level and has population of {self.population} '

# driver code 
def main():
    cities = ["Delhi","New York","London"]
    country = ["India","USA","England"]
    elevations = [216,10,11]
    populations = [31181, 88793, 94252]
    print(f'{City.__doc__}')
    city = []
    for i in range(3):
        city.append(City(cities[i],country[i],elevations[i],populations[i]))
    
    for i in range(len(city)):
        print(f'{city[i]}')
    
    for i in range(len(city)):
        min_pop = int(input("enter the minimum population to check which city from which country suits that population : "))
        print(f'{city[i].max_elevation_city(min_pop,city[2],city[1],city[0])}')
    
if __name__ == "__main__":
    main()
    

# output : 
#    
# this City class has different attribute for a city like city Name, county of the city , elevation
 
# from sea level and the population of that city  and we are using a max_elevation_city function which takes a minimum_population by user checks whether that kind of city is available 

#  with minimum that much populations and have maximum elevation

# Delhi city of India is elevated 216m from sea level and has population of 31181 
# New York city of USA is elevated 10m from sea level and has population of 88793 
# London city of England is elevated 11m from sea level and has population of 94252 


# enter the minimum population to check which city from which country suits that population : 
# 100000
# London, England


# enter the minimum population to check which city from which country suits that population : 
# 17000
# Delhi, India


# enter the minimum population to check which city from which country suits that population : 
# 35689
# London, England
```



Question 5: 
We have two pieces of furniture: a brown wood table and a red leather couch. Create each Furniture class with attributes color, material instance, so that the describe_furniture function can format a sentence that describes these pieces as follows: "This piece of furniture is made of {color} {material}". Use docstring to document the class well. Use __str__ to print a meaningful object description. 


Ans : 
```
class Furniture:
    ''' in this class we initialise the Furniture with the attribute like color and material and then print the format '''
    def __init__(self,color,material):
        self.color = color
        self.material = material
    
    # method for description of furniture
    def describe_furniture(self):
        print(f'the furniture is {self.color} in color and {self.material} material')
    
    def __str__(self):
        print(f'the furniture has attribute color: {self.color} and material : {self.material}')


# driver code
def main():
    Table = Furniture("brown","wood")
    Sofa = Furniture("Black","Fabric ")
    print(f'{Furniture.__doc__}')
    Table.describe_furniture()
    Sofa.describe_furniture()

if __name__ == "__main__":
    main()
    
    
# output : 
# In this class we initialise the Furniture with the attribute like color and material and then print the format
# the furniture is brown in color and wood material
# the furniture is Black in color and Fabric  material

```

Question 6 : 
Write a Person class that has an attribute “name”, which gets set when constructing the object. The class also has the greeting() method is called, the greeting states the assigned name. Use docstring to document the class well. Use __str__ to print a meaningful object description.

Ans : 
```
class Person:
    ''' the class Person descibes the assigned named for the person  '''
    def __init__(self,name):
        self.name = name
    
    # Greeting method for assigned name 
    def Greeting(self):
        print(f'the assigned name is : {self.name}')
    
    def __str__(self):
        return f'the person was assigned the name {self.name}'

# driver code 
def main():
    name = input("enter the name of the person you want to assign : ")
    person1 = Person(name)
    print(f'{Person.__doc__}')
    person1.Greeting()
    
if __name__ == "__main__":
    main()


# output : 
 
# enter the name of the person you want to assign: Ashish
# the class Person describes the assigned named for the person
# the assigned name is : Ashish

```

Question 7: 
Create a Die class with one integer instance variable called sideUp. Give it a constructor and a getSideUp( ) method that returns the value of sideUp and a void roll( ) method that changes sideUp to a random value from 1 to 6. Then creates two Die objects, rolls them, and prints the sum of the two sides up. Use docstring to document the class well. Use __str__ to print a meaningful object description. 


Ans : 
```
import random
class Dice:
    ''' the class is to add the random values to two dices and it initialised at the starting'''
    def __init__(self,SideUp):
        self.SideUp = SideUp
    
    # method to find the number of the dice 
    def getSideUp(self):
        return self.SideUp
    
    # method for giving random number between 1 to 6 
    def roll(self):
        self.SideUp = random.randint(1,6)
    
    def __str__(self):
        return f'the value on the top of the dice is {self.SideUp}'

# driver code 
def main():
    dice1 = Dice(1)
    dice2 = Dice(2)
    print(f'{Dice.__doc__}')
    print(f'{dice1.getSideUp()} value on dice1')
    dice2.getSideUp()
    print(f'{dice2.getSideUp()} value on dice2')
    print(f'now adding the random of the dice : ' )
    dice1.roll()
    print(f'{dice1.getSideUp()} value assigned to dice1 on random')
    dice2.roll()
    print(f'{dice2.getSideUp()} value assigned to dice2 on random')
    print(f'the sum is {dice1.getSideUp()+dice2.getSideUp()} ')

if __name__ == "__main__":
    main()
    
# Output : 


#  the class is to add the random values to two dices and it initialise at the starting
# 1 value on dice1
# 2 value on dice2
# now adding the random of the dice:
# 5 value assigned to dice1 on random
# 6 value assigned to dice2 on random
# the sum is 11

```

Question 8:
Create a Card class that represents a playing card. It should have an int instance variable named rank and a char variable named suit. Give it a constructor with two parameters for initializing the two instance variables and give it a getSuit( ) method and a getRank( ) method that return the values of the two instance variables. Then creates five Cards that make up a full house (that is, three of the cards have the same rank and the other two cards have the same rank) and prints out the ranks and suits of the five Cards using the getSuit( ) and getRank( ) methods. Use docstring to document the class well. Use __str__ to print a meaningful object description. 


Ans : 
```
class Card:
    ''' This Class is used to Show the rank And suit of any given card using two method getSuit and getRank'''
    def __init__(self,rank,suit):
        self.rank = rank
        self.suit = suit
    
    # method to getSuit 
    def getSuit(self):
        return self.suit
    
    # method to getRank
    def getRank(self):
        return self.rank
    
    def __str__(self):
        return f'the rank of the card is : {self.rank} and suit is {self.suit}'


# driver code 
def main():
    print(f'{Card.__doc__}')
    card1 = Card(3, '♥')
    print(f'the rank of the card is {card1.getRank()} and suit is {card1.getSuit()}')
    card2 = Card(3, '♠')
    print(f'the rank of the card is {card2.getRank()} and suit is {card2.getSuit()}')
    card3 = Card(3, '♦')
    print(f'the rank of the card is {card3.getRank()} and suit is {card3.getSuit()}')
    card4 = Card(2, '♦')
    print(f'the rank of the card is {card4.getRank()} and suit is {card4.getSuit()}')
    card5 = Card(2, '♣')
    print(f'the rank of the card is {card5.getRank()} and suit is {card5.getSuit()}')
    
if __name__ == "__main__":
    main()
    

# output : 
#  This Class is used to Show the rank And suit of any given card using two method getSuit and getRank
# the rank of the card is 3 and suit is ♥
# the rank of the card is 3 and suit is ♠
# the rank of the card is 3 and suit is ♦
# the rank of the card is 2 and suit is ♦
# the rank of the card is 2 and suit is ♣
 ```   
    

Question 9:
Create a Swapper class with two integer instance variables x and y and a constructor with two parameters that initialize the two variables. Also include three methods: A getX( ) method that returns x, a getY( ) method that returns y, and a void swap( ) method that swaps the values of x and y. Write instructions to tests all the methods. Use docstring to document the class well. Use __str__ to print a meaningful object description. 

Ans : 
```
class Swapper:
    ''' here this class is used to swap the value of x and y and method to fetch value of x and y '''
    def __init__(self,x,y):
        self.x = x
        self.y = y
    
    # method to get the value of x 
    def getX(self):
        return self.x 
    
    # method to get the value of y 
    def getY(self):
        return self.y
    
    # method to swap values 
    def swap(self):
        temp = self.x 
        self.x = self.y
        self.y = temp 
    
    def __str__(self):
        return f'the value of x : {self.x} and y : {self.y}'
def main():
    point1 = Swapper(1,2)
    print(f'{Swapper.__doc__}')
    print(f'the x value is : {point1.getX()} and y is : {point1.getY()}')
    point1.swap()
    print(f'the x value is : {point1.getX()} and y is : {point1.getY()}')
    
if __name__ == "__main__":
    main()

# output : 
#  here this class is used to swap the value of x and y and method to fetch value of x and y
# the x value is: 1 and y is : 2
# the x value is: 2 and y is : 1
```

Question 10 : 
Create a USMoney class with two integer instance variables dollars and cents. Add a constructor with two parameters for initializing a USMoney object. The constructor should check that the cents value is between 0 and 99 and, if not, transfer some of the cents to the dollars variable to make it between 0 and 99. Add a plus method to the class that takes a USMoney object as its parameter. It creates and returns a new USMoney object representing the sum of the object whose plus( ) method is being invoked and the parameter. It does not modify the values of the two existing objects. It should also ensure that the value of the cents instance variable of the new object is between 0 and 99. For example, if x is a USMoney object with 5 dollars and 80 cents, and if y is a USMoney object with 1 dollar and 90 cents, then x.plus(y) will return a new USMoney object with 7 dollars and 70 cents. Also, write instruction that tests the USMoney class. Use docstring to document the class well. Use __str__ to print a meaningful object description.


Ans : 

```
class USMoney:
    ''' the USMoney is used to initialise dollar and cent and it has add function where it add the two money i.e two object ''' 
    def __init__(self,dollar,cent):
        if cent<0:
            self.cent += 100
            self.dollar -= 1 
        elif cent>99 :
            self.cent -= 100
            self.dollar += 1 
        else :
            self.cent = cent
            self.dollar = dollar
        
        
    # method to add the  money of two object and store it in third variable 
    def plus(self,money):
        m = USMoney(0,0)
        m.cent = self.cent+money.cent
        m.dollar = self.dollar + money.dollar
        if(m.cent>99):
            m.cent -= 100
            m.dollar += 1 
        return m
    def __str__(self):
        return f'we have {self.dollar} dollar and {self.cent}'

# driver code 
def main():
    print(f'{USMoney.__doc__}')
    money1 = USMoney(4,59)
    print(f'{money1.__str__()}')
    money2 = USMoney(5,89)
    print(f'{money2.__str__()}')
    money = USMoney(0,0)
    money = money2.plus(money1)
    print(f'{money.__str__()}')

if __name__ == '__main__':
    main()

# output : 
#        
#  the USMoney is used to initialise dollar and cent and it has add function where it add the two money i.e two object 
# we have 4 dollar and 59
# we have 5 dollar and 89
# we have 10 dollar and 48
```

--------------------------------------------------------------------------------------------------------------------------

Question 11: 
Create a Date class with three integer instance variables named day, month, year. It has a constructor with three parameters for initializing the instance variables, and it has one method named daysSinceJan1( ). It computes and returns the number of days since January 1 of the same year, including January 1 and the day in the Date object. For example, if day is a Date object with day = 1, month = 3, and year = 2000, then the call day.daysSinceJan1( ) should return 61 since there are 61 days between the dates of January 1, 2000, and March 1, 2000, including January 1 and March 1. Include instructions that tests the Date class. Don’t forget leap years. Use docstring to document the class well. Use __str__ to print a meaningful object description. 


Ans : 
```
class Date :
    ''' the Date class is used to initialise the date and along with that it also find the number of days 
    from the very first day of the year '''
    def __init__(self,day,month,year):
        self.day = day
        self.month = month
        self.year = year
    
    # method to count the number of days between the given date and first day of year(inclusive)
    def daysSinceJan1(self):
        leap = 0
        if (self.year%400 == 0):
            leap = 1
        elif self.year%4 == 0 : 
            if self.year%100 != 0: 
                leap = 1
        noOfDays = 0 
        m1 = self.month-1
        while m1 >= 1:
            if  m1 % 2 == 1:
                if m1<=7:
                    noOfDays += 31
                else : 
                    noOfDays += 30
            elif m1 == 2:
                if leap :
                    noOfDays += 29
                else :
                    noOfDays += 28 
            elif m1%2 == 0:
                if m1>=8:
                    noOfDays += 31
                else : 
                    noOfDays += 30
            m1 -= 1
        noOfDays += self.day
        return noOfDays
    
    def __str__(self):
        return f'the date is {self.day} day of month {self.month} and year {self.year} '

# driver code 
def main():
    date1 = Date(1,3,2000)
    print(f'{Date.__doc__}')
    print(f'{date1.__str__()}')
    print(f'the number of days are {date1.daysSinceJan1()}')
    
if __name__ == '__main__':
    main()
        
        
# output: 
 
#  the Date class is used to initialise the date and along with that it also find the number of days 
#  from the very first day of the year 
# the date is 1 day of month 3 and year 2000 
# the number of days are 61

```

Question 12 :
Create a Person class with instance variables for the person’s name and birth date. Then create a subclass CollegeGraduate with instance variables for the student’s GPA and year of graduation. Don’t forget to include appropriate constructors for your classes. Include instructions that tests the class. Use docstring to document the class well. Use __str__ to print a meaningful object description. 

Ans : 
```
class Person() :
    ''' this class is about the information of the student name and date of birth '''
    def __init__(self, name , dob):
        self.name = name
        self.dob = dob
  
# this is the subclass of class "Person"
class CollegeGraduate(Person):
    ''' This is a subclass for person where the student is in which year of Graduation and his/her GPA'''
    def __init__(self, name , dob , gpa , year):
        super().__init__(name,dob)
        self.gpa = gpa
        self.year = year
    def __str__(self):
        return f'{self.name} with Date Of Birth {self.dob} is in {self.year} in Graduation with GPA of : {self.gpa}'
def main():
    print(f'{Person.__doc__}')
    print(f'{CollegeGraduate.__doc__}')
    student = CollegeGraduate("Ashish Kumar" , "24/11/2001 ", 2 , 8.0 )
    print(f'{student.__str__()}')
if __name__ == '__main__':
    main()

# output : 

#    
#  this class is about the information of the student name and date of birth 
#  This is a subclass for person where the student is in which year of Graduation and his/her GPA
# Ashish Kumar with Date Of Birth 24/11/2001  is in 2 year in Graduation with GPA of : 8.0
```
