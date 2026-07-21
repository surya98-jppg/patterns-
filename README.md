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
    for j in range(i+1):             when row =0 stars =1 means i=0 outer (inner = i+1) 
        print("*",end = "")
    print()
output
*
**
***
****
*****
