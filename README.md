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

# Half pyramid(floyd's triangle)
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
output                               if we want 5555 4444,333 we use n-i to print
****  
***                                 j has values 0 1 2 3 in the program first inner executes the                       **                                code      **                                    inside it
*
# full pyramid(pascals triangle)
n=5
for i in range(n):
    for j in range(n-i-1):
        print(" ",end="")
    for j in range(2*i+1):
           if i==n-1:
            print("+",end="")
           else:
               print("*",end="")
    print()
ouput
    *                                    if we want specific to print another we use this
   ***
  *****
 *******
+++++++++

# Reverse  pyramid
n=int(input("ennter a number"))
for i in range(n):
    for j in range(i):
        print(" ",end="")
    for j in range(2*(n-i)-1):
          print(2*(n-i)-1,end="")
    print()
output:
999999999
 7777777
  55555
   333
    1
# Diamond pattern
n=5
#for top pattern
for i in range(n):
    for j in range(n-i-1):
      print(" ",end="")
    for j in range(2*i+1):
        print(chr(65+i),end="")
    print()
#for bottom
for i in range(1,n):
    for j in range(i):
        print(" ",end="")
    for j in range(2*(n-i)-1):
        print(chr(65+n-i-1),end="")
    print()
 
#to avoid printing of last row in top twotimes we start thr bottom loop from (1,n) instead of (0,n)
output:-
    A
   BBB
  CCCCC
 DDDDDDD
EEEEEEEEE
 DDDDDDD
  CCCCC
   BBB
    A
# hollow sqaure
n=int(input("enter  number"))
for i in range(n):
     for j in range(n):
         if i==0 or i==n-1 or j==0 or j==n-1:
             print("*",end="")
         else:
             print(" ",end="")
     print()
     # first assume a matrix of hollow sqaure  print the stars where stars present otherwise print spaces
output:
****
*  *
*  *
****
# Hollow pyramid
n=5
for i in range(n):
    for j in range(n-i-1):
        print(" ",end="")
    for j in range(2*i+1):                    in this j=0 prints firsr and j=2*i prints last coloumn
        if j==0 or j==2*i or i==n-1:
            print(chr(65+i),end="")
        else:
            print(" ",end="")
    print()
outut
   A
   B B
  C   C
 D     D
EEEEEEEEE

# Butterfly pattern
n=int(input("enter a number"))
for i in range(n):
    
    for j in range(i+1):
        print("*",end=" ")
    for j in range(2*(n-i-1)):
        print(" ",end=" ")
    for j in range(i+1):
        print("*",end=" ")
    print()
    
for i in range(1,n):                                          divide the pattern into two halves then check what to print
    
    for j in range(n-i):
        print("*",end=" ")
    for j in range(2*i):
        print(" ",end=" ")
    for j in range(n-i):
        print("*",end=" ")
    print()

output
*             * 
* *         * * 
* * *     * * * 
* * * * * * * * 
* * *     * * * 
* *         * * 
*             * 

# Hollow Diamond
 n=5
for i in range(n):
    for j in range(n-i-1):
        print(" ",end="")
    for j in range(2*i+1):
        if j==0 or j==2*i:
            print("*",end="")
        else:
            print(" ",end="")
    print()

for i in range(1,n):
    for j in range(i):
        print(" ",end="")
    for j in range(2*(n-i)-1):
        if j==0 or j==2*(n-i)-2:
            print("*",end="")
        else:
            print(" ",end="")
    print()
output
    *
   * *
  *   *
 *     *                     for leading spaces we use the first j loop for spaces inside the diamond we use the second j loop
*       *
 *     *
  *   *
   * *
    *  
# Floyod triangle
n=int(input("enter a number"))
num=1
for i in range(n):
    for j in range(i+1):
        print(num,end=" ")
        num+=1
    print()
floyd's Triangle is a number pattern in which consecutive numbers are printed in a triangular form, with the i-th row containing i numbers (or i+1 numbers if using 0-based indexing), and the numbers continue without resetting.
output:-
1 
2 3 
4 5 6 
7 8 9 10 
11 12 13 14 15 
# reverse floyd triangle
n=int(input("enter a number"))
total=n*(n+1)//2
current=total
for i in range(n,0,-1):
    for j in range(i):
        print(current,end=" ")
        current-=1
    print()
output
15 14 13 12 11 
10 9 8 7 
6 5 4 
3 2 
1 
# Pascal Triangle
n=4
for i in range(n):
    for j in range(n-i-1):
        print(" ",end="")
    value=2
    for j in range(i+1):
      print(value,end="")
      value=value*(i-j)//(j+1)
    print()
output:
   1
   11
  121
 1331
14641
# reverse pascal triangle
n = int(input("Enter rows: "))
for i in range(n):
    for j in range(2*i):
        print(" ",end="")
    row=n-i-1
    value=1
    for j in range(row+1):
        print(value,end="")
        value=value*(row-j)//(j+1)
    print()
output:
14641
  1331
    121
      11
        1
# Alphabet floyod triangle
n=int(input("enter a number"))
ch=65
for i in range(n):
     for j in range(i+1):
         print(chr(ch),end="")
         ch+=1
     print()
output:
A 
B C 
D E F 
G H I J 
K L M N O
# palindromic alphabetic pattern
n=5
for i in range(n):
    for j in range(i+1):
        print(chr(65+j),end="")
    for j in range(i-1,-1,-1):
        print(chr(65+j),end="")
    print()
output
A
ABA
ABCBA
ABCDCBA
ABCDEDCBA
# Centered aplhabet palindromic pyramid(repeation of alphabet pattern)
n=5
for i in range(n):
    for j in range(n-i-1):
        print(" ",end="")
    for j in range(i+1):
        print(chr(65+j),end="")
    for j in range(i-1,-1,-1):
        print(chr(65+j),end="")
    print()
output:
    A
   ABA
  ABCBA
 ABCDCBA
ABCDEDCBA
# Inverted centered palindromic alphabet pyramid
n=int(input("enter a number"))
for i in range(n):
    for j in range(i):
        print(" ",end="")
    for j in range(n-i):
        print(chr(65+j),end=" ")
    for j in range(n-i-2,-1,-1):
        print(chr(65+j),end=" ")
    print()
output:
A B C D E D C B A 
 A B C D C B A 
  A B C B A 
   A B A 
     A 
# medium question
n=5
for i in range(n):
    for j in range(i):
        print(" ",end="")
    start=65+n-i-1
    for j in range(n-i):
        print(chr(start-j),end="")
    print()
output:
E D C B A 
  D C B A 
    C B A 
      B A 
        A 
# hard question
=5
for i in range(n):
    for j in range(i):
        print(" ",end="")
    for j in range(i,n):
        print(chr(65+j),end="")
    for j in range(n-2,i-2,-1):
        print(chr(65+j),end="")
    print()
output
ABCDEDCBA@
 BCDEDCBA
  CDEDCB
   DEDC
    ED

        
