# Basic-python-programs
10-02-2025
1. Basic python programs 
1.Program or script which demonstrates the use of different datatypes.
a=12
print(a)
print(type(a))
output:
12
<class 'int'>
 
a='appu'
print(a)
print(type(a))
 
output:
appu
<class 'str'>
 
a=3.12
print(a)
print(type(a))
output:
3.12
<class 'float'>
2.Program to make use of following operators
Arithmetic operations , logical operations and relational operations.
  a = 25
 b = 10
 sum_result = a + b
print(f"Sum: {a} + {b} = {sum_result}")
subtraction_result = a - b
print(f"Subtraction: {a} - {b} = {subtraction_result}")
 output:
Sum: 25 + 10 = 35
Subtraction: 25 - 10 = 15
3.Program to make use of ifelse and nested ifelse loops.
a. Finding biggest of three numbers  
 a=int(input(“enter a number:”))
b= int(input(“enter a number:”))
c= int(input(“enter a number:”))
if(a>b and a>c):
print(a,’is greatest’)
elif(b>a and b>c):
print(b,’is greatest’)
elif(c>a and c>b):
print(c,’is greatest’)
else:
print(’all are equal’)
Output:
enter a number:56
enter a number:47
enter a number:100
100 is greatest
B.even or odd 
num = int(input("Enter a number: "))
if num % 2 == 0:
    print(f"{num} is Even")
else:
    print(f"{num} is Odd")
Output:
Enter a number: 45
45 is Odd

C. prime number 
def is_prime(n):
    if n < 2:
        return False
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return False
    return True
num = int(input("Enter a number: "))
if is_prime(num):
    print(f"{num} is a prime number.")
else:
    print(f"{num} is not a prime number.")

Output:
Enter a number: 41
41 is a prime number.
4.Program to make use of while loop
a. Print the series from 1 to n
n = int(input("Enter a number: "))
i = 1
while i <= n:
    print(i, end=" ")
    i += 1

Output:
Enter a number: 5
1 2 3 4 5
b. Print the even or odd series
n = int(input("Enter a number: "))
i = 1
print("Even numbers:")
while i <= n:
    if i % 2 == 0:
        print(i, end=" ")
    i += 1
i = 1
print("\nOdd numbers:")
while i <= n:
    if i % 2 != 0:
        print(i, end=" ")
    i += 1
Output:
Enter a number: 44
Even numbers:
2 4 6 8 10 12 14 16 18 20 22 24 26 28 30 32 34 36 38 40 42 44 
Odd numbers:
1 3 5 7 9 11 13 15 17 19 21 23 25 27 29 31 33 35 37 39 41 43
c.sum of natural numbers 
n = int(input("Enter a number: "))
sum = 0
i = 1
while i <= n:
    sum += i
    i += 1
print(f"Sum of first {n} natural numbers is {sum}")
Output:
Enter a number: 5
Sum of first 5 natural numbers is 15
d.armstrong number 
num = int(input("Enter a number: "))
sum = 0
temp = num
order = len(str(num))
while temp > 0:
    digit = temp % 10
    sum += digit ** order
    temp //= 10
if num == sum:
    print(f"{num} is an Armstrong number.")
else:
    print(f"{num} is not an Armstrong number.")
Output:
Enter a number: 153
153 is an Armstrong number.
e.palindrome 
num = int(input("Enter a number: "))
temp = num
rev = 0
while temp > 0:
    digit = temp % 10
    rev = rev * 10 + digit
    temp //= 10
if num == rev:
    print(f"{num} is a palindrome.")
else:
    print(f"{num} is not a palindrome.")
Output:
Enter a number: 121
121 is a palindrome.
5.Program to make use of for loop
n=int(input(“Enter the range of sum\n”)
sum=0
For i in range(n+1):
sum+=i
print(‘Sum of’,n,’number is:’,sum)
Output:
Enter the range of sum
11
Sum of 11 number is: 66

6.Program which demonstrates the use of function following
      a. 	No values passing and no parameters return
def greet():
    print("Hello! Welcome to Python functions.")
greet()
Output:
Hello! Welcome to Python functions.
  b. Passing values and no parameters returns
def greet(name):
    print(f"Hello, {name}! Welcome to Python functions.")
greet("Alice")
Output:
Hello, Alice! Welcome to Python functions.
  c.  No passing values but return types
def get_message():
    return "Hello! This is a returned message."

message = get_message()
print(message)
Output:
Hello! This is a returned message.
 d. Parameters passing and return types
def add_numbers(a, b):
    return a + b
result = add_numbers(5, 7)
print(f"The sum is: {result}")
Output:The sum is: 12





7.Program to make use of lists and their operations or methods.
l1=[1,2,3]
l1
l2=[1.5,1.2]
l2
l3=['a','b']
l3
l4=['apple']
l4
output:
['apple']
 
 
l1=[1,2,3]
print(l1)
l2=[1.5]
print(l2)
l1
output:
[1, 2, 3]
[1.5]
[1, 2, 3]
 
 
l1=[1,2,3]
print(l1)
l2=[1.5]
print(l2)
l1
l2
 
output:
[1, 2, 3]
[1.5]
[1.5]
 
 
 
l1=[1,2,3]
l1.extend([20,50])
print(l1)
 
output:
[1, 2, 3, 20, 50]
 
 
 
 
l1=[1,2,3]
l1.extend([20,50])
print(l1)
l1.append(50)
print(l1)
 
output:
[1, 2, 3, 20, 50]
[1, 2, 3, 20, 50, 50]
 
 
l1=[1,2,3]
l1.extend([20,50])
print(l1)
l1.append(50)
print(l1)
l1.insert(1,20)
print(l1)
 
output:
[1, 2, 3, 20, 50]
[1, 2, 3, 20, 50, 50]
[1, 20, 2, 3, 20, 50, 50]
 
 
l1=[1,2,3]
l1.extend([20,50])
print(l1)
l1.append(50)
print(l1)
l1.insert(1,20)
print(l1)
l1.pop()
print(l1)
l1.remove(2)
print(l1)
 
output:
 
[1, 2, 3, 20, 50]
[1, 2, 3, 20, 50, 50]
[1, 20, 2, 3, 20, 50, 50]
[1, 20, 2, 3, 20, 50]
[1, 20, 3, 20, 50]
 
 
 
l1=[1,2,3]
l1.extend([20,50])
print(l1)
l1.append(50)
print(l1)
l1.insert(1,20)
print(l1)
l1.pop(3)
print(l1)
l1.remove(2)10
print(l1)
 
output:
[1, 2, 3, 20, 50]
[1, 2, 3, 20, 50, 50]
[1, 20, 2, 3, 20, 50, 50]
[1, 20, 2, 20, 50, 50]
[1, 20, 20, 50, 50}
8.Program to make use of dictIonaries and their methods

 a={‘01’: ‘dhruv’, ‘02’ : ‘tarun’}
print(a)
print(type(a))
print(len(a))
print(a| ‘02’ |)
print(a.get( ‘02’))
k=a.keys()
print(k)
v=a.values()
print(v)
x=a.items()
print(x)
If ‘02’ in a :

 print(‘yes’)
a.update({‘03’ : ‘asheer’})
print(x)
Output:
{‘01’ : ‘dhruv’,’02’ : ‘tarun’}
<class ‘dict’>
2
tarun
tarun
dict_keys([‘01’ , ‘02’])
dict_values([‘dhruv’ , ‘tarun’])
dict_items([‘01’ , ‘dhruv’),(‘02’,’tarun’)])
Yes
dict_items([‘01’ , ‘dhruv’),(‘02’,’tarun’),(‘03’,’asheer’)])
9. program to make use of tuples and their methods.
names=(‘A’,’B’,’C’,’D’)
print(names)
print(type(names))
name=list(names)
name.append(‘E’)
print(name)
print(type(name))
names=tuple(name)
days=(‘sunday’, ‘monday’, ‘tuesday’)
days2=(‘wednesday’, ‘thursday’, ‘friday’)
days=days+days2
print(days)
days=(‘sunday’, ‘monday’, ‘tuesday’)
(first,second,third)=days
print(days)
print(first)
print(second)
print(third)
print(names)
print(names.count(‘A’))
print(names)
print(names. index(‘C’))
Output:
(‘A’,’B’,’C’,’D’)
<class ‘tuple’>
[‘A’,’B’,’C’,’D’ ,’E’]
<class ‘list’>
(‘sunday’,’monday’,’tuesday’,’wednesday’,’thursday’,’friday’)
(‘sunday’,’monday’,’tuesday’)
sunday
monday
tuesday
(‘A’,’B’,’C’,’D’,’E’)
1
(‘A’,’B’,’C’,’D’,’E’)
2
10.  Program to make use of sets and their operations
# Define two sets
set_a = {1, 2, 3, 4, 5}
set_b = {4, 5, 6, 7, 8}
print("Set A:", set_a)
print("Set B:", set_b)
# Union
union_set = set_a | set_b
print("\nUnion:", union_set)
# Intersection
intersection_set = set_a & set_b
print("Intersection:", intersection_set)
# Difference (elements in set_a but not in set_b)
difference_set = set_a - set_b
print("Difference (A - B):", difference_set)
# Symmetric Difference (elements in either set but not both)
symmetric_difference_set = set_a ^ set_b
print("Symmetric Difference:", symmetric_difference_set)
Output:
Set A: {1, 2, 3, 4, 5}
Set B: {4, 5, 6, 7, 8}
Union: {1, 2, 3, 4, 5, 6, 7, 8}
Intersection: {4, 5}
Difference (A - B): {1, 2, 3}
Symmetric Difference: {1, 2, 3, 6, 7, 8}




