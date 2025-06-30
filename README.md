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

