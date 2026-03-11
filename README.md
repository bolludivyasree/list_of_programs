# list_of_programs

1️⃣ Basic Programming & Logic (30 Programs)
Hello World

Even or Odd number

Largest of two numbers

Largest of three numbers

Swap two numbers

Sum of N natural numbers

Factorial of number

Prime number

Armstrong number

Palindrome number

Fibonacci series

Reverse number

Sum of digits

Count digits

GCD of two numbers

LCM of two numbers

Perfect number

Multiplication table

Power of number

Check leap year

Simple calculator

Sum of array elements

Average of numbers

Find max element

Find min element

Reverse array

Check palindrome string

Reverse string

Count vowels

Pattern printing

2️⃣ Arrays (30 Programs)
Find largest element

Find smallest element

Reverse array

Rotate array left

Rotate array right

Second largest element

Remove duplicates

Move zeros to end

Merge two arrays

Find intersection

Find union of arrays

Find missing number

Find duplicates

Maximum subarray sum (Kadane’s)

Find equilibrium index

Rearrange positive and negative

Count pairs with given sum

Product of array except self

Leaders in array

Stock buy and sell

Trapping rain water

Maximum product subarray

Subarray with given sum

Longest consecutive sequence

Rotate matrix

Spiral matrix

Search element in matrix

Find majority element

Find kth largest element

Minimum jumps to reach end

3️⃣ Strings (20 Programs)
Reverse string

Palindrome string

Count vowels and consonants

Remove duplicates

Find duplicate characters

Anagram check

Longest word in sentence

Remove spaces

Count words

First non-repeating character

String compression

Check substring

Longest common prefix

Reverse words in sentence

String rotation

Longest substring without repeating characters

Check valid parentheses

Print all substrings

Find frequency of characters

Replace characters

4️⃣ Recursion (20 Programs)
Factorial using recursion

Fibonacci using recursion

Sum of numbers using recursion

Reverse string

Reverse array

Power of number

Sum of digits

Binary search recursion

Tower of Hanoi

Generate subsets

Generate permutations

Nth Fibonacci number

Print numbers from 1 to N

Print numbers N to 1

Check palindrome

Find max element recursively

Count ways to climb stairs

Generate combinations

Print all subsequences

Parenthesis combinations

5️⃣ Searching Algorithms (15 Programs)
Linear search

Binary search

Recursive binary search

Find first occurrence

Find last occurrence

Count occurrences

Search in rotated array

Find peak element

Jump search

Interpolation search

Exponential search

Search in matrix

Find floor element

Find ceil element

Find closest element

6️⃣ Sorting Algorithms (15 Programs)
Bubble sort

Optimized bubble sort

Selection sort

Insertion sort

Merge sort

Quick sort

Heap sort

Counting sort

Radix sort

Bucket sort

Sort 0,1,2 array

Sort characters in string

Kth smallest element

Merge two sorted arrays

Sort nearly sorted array

7️⃣ Linked List (20 Programs)

Create linked list

Insert node at beginning

Insert node at end

Insert node at position

Delete node at beginning

Delete node at end

Delete node by value

Traverse linked list

Search element

Find length

Reverse linked list

Find middle node

Detect loop

Remove loop

Merge two lists

Remove duplicates

Find nth node from end

Rotate linked list

Palindrome linked list

Intersection of two lists

8️⃣ Stack (15 Programs)
Implement stack using array

Implement stack using linked list

Push operation

Pop operation

Peek operation

Reverse string using stack

Balanced parentheses

Evaluate postfix expression

Infix to postfix

Infix to prefix

Next greater element

Stock span problem

Min stack

Sort stack

Reverse stack using recursion

9️⃣ Queue (15 Programs)
Implement queue using array

Implement queue using linked list

Enqueue operation

Dequeue operation

Circular queue

Priority queue

Deque implementation

Reverse queue

Queue using two stacks

Stack using two queues

First non-repeating character in stream

Sliding window maximum

Reverse first K elements

Interleave queue

Generate binary numbers

🔟 Trees (20 Programs)
Create binary tree

Inorder traversal

Preorder traversal

Postorder traversal

Level order traversal

Height of tree

Count nodes

Count leaf nodes

Find max element

Search element

Check balanced tree

Diameter of tree

Lowest common ancestor

Mirror tree

Check identical trees

Boundary traversal

Zigzag traversal

Vertical traversal

Binary search tree check

Convert tree to mirror

1️⃣1️⃣ Graphs (15 Programs)
Graph adjacency matrix

Graph adjacency list

BFS traversal

DFS traversal

Detect cycle

Topological sort

Dijkstra algorithm

Bellman-Ford algorithm

Floyd-Warshall algorithm

Prim’s MST

Kruskal’s MST

Connected components

Bipartite graph check

Strongly connected components

Shortest path BFS

1️⃣2️⃣ Dynamic Programming (20 Programs)

Fibonacci DP

Climbing stairs

Coin change

0/1 knapsack

Longest common subsequence

Longest increasing subsequence

Longest palindromic subsequence

Edit distance

Matrix chain multiplication

Minimum path sum

Rod cutting problem

Word break problem

Maximum subarray sum

Unique paths grid

Egg dropping problem

Catalan numbers

House robber problem

Partition subset sum

Minimum cost climbing stairs

Maximum product subarray



# Sum of N natural numbers

n=int(input())
sum=0
for i in range(n+1):
    sum=sum+i
print(sum)

output:
input value: 10
55

# Factorial of number

n=int(input())
fact=1
for i in range(1, n+1):
    fact=fact*i
print(fact)

output: 
input value: 5
120

# Prime number

n=int(input("Enter a number: "))
flag=0
if n<=1:
    flag=1
for i in range(2,n):
    if(n%i==0):
        flag=1
        break
if flag==0:
    print(f"{n} is Prime Number")
else:
    print(f"{n} is not Prime Number")


n = int(input("Enter number: "))
flag = 0

if n <= 1:
    flag = 1
else:
    for i in range(2, n//2 + 1):
        if n % i == 0:
            flag = 1
            break

if flag == 0:
    print(n, "is Prime")
else:
    print(n, "is not Prime")

output: 
Enter a number: 47
it is a prime

# Armstrong number

n=int(input("Enter a number: "))
temp=n
length=len(str(n))
sum=0
while n!=0:
    rem=n%10
    sum=sum+rem**length
    n=n//10
if temp==sum:
    print("Armstrong Number")
else:
    print("Not Armstrong")
    
Output: 
Enter a number: 153
Armstrong Number


# Palindrome number

n=int(input("Enter a number"))
temp=n
rev=0
while n!=0:
    rem=n%10
    rev=rev*10+rem
    n=n//10
if temp==rev:
    print("Palindrome")
else:
    print("Not Palindrome")

output:
Enter a number: 1221
Palindrome

# Fibonacci series
n=int(input())
a,b=0,1
print(a,b, end=" ")
for i in range(2,n):
    c=a+b
    print(c,end=" ")
    a,b=b,c
    
output:
10
0 1 1 2 3 5 8 13 21 34 

#  Reverse number
n=int(input())
rev=0
while n!=0:
    rem=n%10
    rev=rev*10+rem
    n=n//10
print(rev)

output:
123456
654321

# Sum of digits
n=int(input())
sum=0
while n!=0:
    rem=n%10
    sum=sum+rem
    n=n//10
print(sum)

output:
124
7

# Count digits

n=int(input())
count=0
while n!=0:
    count=count+1
    n=n//10
print(count)

output:
12456
5

# GCD of two numbers
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

while b != 0:
   a,b=b,a%b

print("HCF or GCD is:", a)

output:
Enter first number: 12
Enter second number: 18
HCF or GCD is: 6

# LCM of two numbers

a=int(input("Enter a number: "))
b=int(input("Enter a number: "))

temp_a=a
temp_b=b
while temp_b!=0:
    temp_a,temp_b=temp_b,temp_a%temp_b
gcd=temp_a
lcm=(a*b)//gcd
print("LCM: ",lcm)

output:
Enter a number: 4
Enter a number: 6
LCM:  12

# Perfect number

n=int(input("Enter a number: "))
temp=n
sum=0
for i in range(1,n):
    if(n%i==0):
        sum=sum+i
if sum==temp:
    print("Perfect")
else:
    print("Not Perfect")

output:
Enter a number: 6
Perfect

# Multiplication table
n=int(input("Enter a number: "))
for i in range(1,11):
    print(f"{n} * {i} = {n*i}")
    
output:
Enter a number: 20
20 * 1 = 20
20 * 2 = 40
20 * 3 = 60
20 * 4 = 80
20 * 5 = 100
20 * 6 = 120
20 * 7 = 140
20 * 8 = 160
20 * 9 = 180
20 * 10 = 200

# Power of number

a=int(input("Enter a number: "))
b=int(input("Enter Power: "))
print(a**b)


a=int(input("Enter a number: "))
b=int(input("Enter Power: "))
result=1
for i in range(1,b+1):
    result=result*a
print(result)

a = int(input())
b = int(input())

print(pow(a, b))

output:
Enter a number: 20
Enter Power: 3
8000

# Check leap year
year=int(input("Enter year: "))
if ((year%4==0 and year%100!=0) or (year%400==0 or year%100==0)):
    print("Leap Year")
else:
    print("Not Leap Year")

Output:
Enter year: 2004
Leap Year

# Simple calculator

Output:

# Sum of array elements

Output:

# Average of numbers

Output:

# Find max element

Output:

# Find min element

Output:

# Reverse array

Output:

# Check palindrome string

Output:

# Reverse string

Output:

# Count vowels

Output:

# Pattern printing

Output:
