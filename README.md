#question1:From this given string: s = "Hey i am from New Delhi". Find out: length of string, convert this to list using split operation.
ANS: 
s = "Hey i am from New Delhi"
print(len(s))
sp=s.split()
print(sp)

#ques2: Given string s = "name is rahul". Write code to give following o/p.
- "Name is rahul"
-  "Rame Is Rahul"
-  "NAME IS RAHUL"
ANS:
s = "name is rahul"
b='N'+s[1:]
print(b)
c='R'+s[1:8]+'R'+s[9:]
print(c)
print(s.upper())

#ques3:Using length and breadth as input find out area and perimeter of a given rectangle.
ANS:
l=int(input("Length= "))
b=int(input("Breadth= "))
area=l*b
print("Area= ",area)
peri=2*(l+b)
print("Perimeter= ",peri)

#QUES4: Using diameter as input find out circumference and area of a circle.
ANS:
d=float(input("Diameter= "))
r=0.5*d
print("Radius=",r)
PI=3.14
area=PI*r*r
print("Area of circle= ",area)
cir=2*PI*r
print("Circumference of circle= ",cir)

QUES5:Write a program to compute roots of a quadratic equation when coefficients a, b and c are known(entered by user).
ANS:
import math
cofa=float(input("Enter the Coefficient a : "))
cofb=float(input("Enter the Coefficient b : "))
cofc=float(input("Enter the Coefficient c : "))
disc = math.sqrt((cofb**2)-4*(cofa*cofc))
alpha=(-cofb + disc)/2*cofa
beta=(-coffb - disc)/2*cofa
print("The Roots of the Quadratic equation : ", "Alpha = ",alpha, "Beta = ",beta)

QUES6:Find volume of a sphere using radius as input.
ANS:
r=float(input("radius= "))
PI=3.14
vol=1.33*PI*r*r*r
print("Volume of sphere= ",vol)

QUES7:Count the  number of digits in a number. Example: 3454 has 4 digits.
ANS:
n=int(input("Enter the digit:"))
count=0
while(n>0):
 count=count+1
 n=n//10
print("no of digits are",count)

QUES8. Write a program that accepts a string and gives output string with all capital letters.
ANS:
s=str(input("enter a string= "))
print(s.upper())

QUES9. Write a program to that accepts a string s, an index number n and a character ‘c’. And outputs the string replaced with the character at the index number n. Example- ‘hello’ , 0 , ‘j’ ==> ‘jello’.
(Hint2: You can try it by join function too by typecasting it to list)
ANS:
s=input("Enter String : ")
n=int(input("Enter Index : "))
c=input("Enter Character : ")
temp=list(s)
temp[n]=c
s=" ".join(temp)
print(s)

Q10. Reverse a string. Example: 'Hey there' = 'ereht yeH'
ANS:
s="Hey There"[::-1]
print(s)
