# patterns-
# square pattern
n=int(input("enter how many iterations"))
value=int(input("entter a value"))                 
for i in range(n):
    for j in range(n):
        print(value,end ="")
    print()  # we can put what ever we cant in the value if we want * to print then "*" etc
output
******
******
******
# Rectangle patterns
for i in range(rows):
    for j in range(cols):
        print(@, end="")
    print()
output
@@@@@@
@@@@@@
@@@@@@
@@@@@@

# Half pyramid
n=int(input("enter a number"))
for i in range(n):
    for j in range(i+1):
        print(i+1,end = "")             when we want output in alphabtes use char(65+i) means
    print()                             chr(65) is A that's why
output
1
22
333
4444
55555
output 2
1
12
123           if we want this change i+1 to j+1(in revrse half is also same)
1234
# Reverse half  pyramid
n=4
for i in range(n):                   in this if i=0 it prints 4 stars then i increases stars decreases so : n-i
    for j in range(n-i):
        print("*",end="")           when i=0 inner loop runs n time upto the condition is false and prints the stars 
    print()
 output                           if we want 5555 4444,333 we use n-i to print
 ****  
***                                 j has values 0 1 2 3 in the program first inner executes the code inside it
**
*
