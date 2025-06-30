# basicfunction-7
code--1::
   #user defined function
def hi():
    print("hello students")
hi()
output::       hello students


code--2:
#user defined function with args.....
def summate(a,b):
    print("sum of two numbers",a+b)
a=int(input("enter the value of a:"))
b=int(input("Enter the value of b:"))
summate(a,b)
output::
enter the value of a:5
Enter the value of b:4
sum of two numbers 9


code3::
#user defined function with args and return values....

def summate(x,y):
    return x+y
a=int(input("enter the value of a:"))
b=int(input("Enter the value of b:"))
#print(summate(a,b))
result=summate(a,b)
print(result)


output::
enter the value of a:6
Enter the value of b:4
10


code4::
#default arg

def power(base,expo=2):
    return base**expo
num=int(input("Enter the base:"))
print(power(num))
print(power(num,3))

output::
Enter the base:3
9
27


code 5::

#multiple return values from a single function

def operate(a,b):
    return a+b, a-b, a*b
a=int(input("Enter a:"))
b=int(input("Enter b:"))
sum,diff,mul=operate(a,b)
print("Sum:",sum)
print("Subtract:",diff)
print("Product:",mul)

output::
Enter a:10
Enter b:5
Sum: 15
Subtract: 5
Product: 50

code6::
#anonumus function lambda
#lambda var: operation

num=int(input("Enter a number:"))
square=lambda num:num*num
print(square(num))

output:::
Enter a number:3
9


or  addition
#anonumus function lambda
#lambda var: operation

num1=int(input("Enter anumber1:"))
num2=int(input("Enter a number2:"))
square=lambda num1,num2:num1+num2
print(square(num1,num2))
output::
Enter anumber1:20
Enter a number2:30
50


code7::

### NESTED FUNCTION()

## nested functions()

def hi():
    def hello():
        print("inner function")
    print("outer function")
    hello()
print("nested function")
hi()

OUTPUT()::
nested function
outer function
inner function


code8::
## nested functions() with operation()


def operation(a,b):
    def add():
        return a+b
    def sub():
        return a-b
    print("Addition :",add())
    print("subtract:",sub())

a=int(input("Enter a:"))
b=int(input("Enter b:"))
operation(a,b)

output::
Enter a:10
Enter b:5
Addition : 15
subtract: 5

code9:: nested fun with fact() and power()
''''write a program to calculate the factorial and power of given numbers by creating the nested loops with in loop
where a=5 & b=3
 calculate the factorial for a 
caulate powere for 5**3 
output::
factorial=120
power=125
'''

code::
def operation(a,b):
    def power(a,b):
        return a**b
    def fact(a):
        op=1
        for i in range(1,a+1):
            op *=i
        return op
    print("Power:",power(a,b))
    print("Factorial:",fact(a))
a=int(input("Enter a:"))
b=int(input("Enter b:"))
operation(a,b)

code10::
factorial func()

def fact(n):
    if n==0:
        return 1
    else:
        return n*fact(n-1)
    
num=int(input("Enter the number:"))
print("Factorial",fact(num))
output::
Enter the number:4
Factorial 24


code11:::

#Recursive functions()
''' fact=4!=4*3*2*1=24
super factorial= 4!=4!*3!*2!*1!=24*6*2*1=288
'''


def fact(n):
    if n==0 or n==1:
        return 1
    return n*fact(n-1)
def sfact(n):
    if n==1:
        return 1
    return fact(n) *sfact(n-1)
    
num=int(input("Enter the number:"))
print("Factorial",sfact(num))

output()::
Enter the number:4
Factorial 288.
