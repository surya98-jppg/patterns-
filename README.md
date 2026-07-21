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
    print()                             char(65) is A that's why
output
1
22
333
4444
55555
output 2
1
12
123           if we want his chane i+1 to j+1
1234

