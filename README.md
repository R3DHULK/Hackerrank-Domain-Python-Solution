![HackerRank Python Solution](./HackerRank%20Python%20Rank.png)

<h1><b>Solutions 👇</h1></b>
<h2><b>Hello World</h2></b>

```
Print ("Hello World")
```

#

<h2><b>Python IF-Else</h2></b>

```
import math, os, random, re, sys

n = int(input())
if n % 2 != 0:
  print("Weird")
else:
  if n >= 2 and n <= 5:
    print("Not Weird")
  elif n >= 6 and n <= 20:
    print("Weird")
  else:
    print("Not Weird")
```

#

<h2><b>Arithmetic operators:</h1></b>

```
a = int(input())
b = int(input())

print(a + b)
print(a - b)
print(a * b)
```

#

<h2><b>Python Divison:</h2></b>

```
if __name__ == '__main__':
    a = int(input())
    b = int(input())

    print(a // b)
    print(a / b)
```

#

<h2><b>Loops:</b></h2>

```
if __name__ == '__main__':
    n = int(input())
    for i in range(n):
        print(i**2)
```

#

<h2><b> Write A Function:   </b></h2>

```
def is_leap(year):
    leap = False
    
    # Write your logic here
    if year % 400 == 0:
        leap = True
    elif year % 100 == 0:
        leap = False
    elif year % 4 == 0:
        leap = True
    
    return leap

year = int(input())
print(is_leap(year))

```


#


<h2><b> Print function:   </b></h2>

```
if __name__ == '__main__':
    n = int(input())
    for i in range(1, n+1):
        print(i, end="")


```


#
<h2><b>  List Comprehensions:  </b></h2>

```

if __name__ == '__main__':
    x = int(input())
    y = int(input())
    z = int(input())
    n = int(input())

    result = [[i, j, k] for i in range(x + 1) for j in range(y + 1) for k in range(z + 1) if i + j + k != n]
    print(result)


```


#
<h2><b> Find The Runner-Up Score:   </b></h2>

```

if __name__ == '__main__':
    n = int(input())
    scores = list(map(int, input().split()))
    scores.sort(reverse=True)
    for i in range(n):
        if scores[i] != scores[0]:
            print(scores[i])
            break

```


#
<h2><b> Nested List:   </b></h2>

```
STUDENTS = []
SECOND_LOWEST_GRADES = []
GRADES = set()

for _ in range(int(input())):
    name = input()
    grade = float(input())
    STUDENTS.append([name, grade])
    GRADES.add(grade)

SECOND_LOWEST = sorted(GRADES)[1]

for name, grade in STUDENTS:
    if grade == SECOND_LOWEST:
        SECOND_LOWEST_GRADES.append(name)

for name in sorted(SECOND_LOWEST_GRADES):
    print(name, end='\n')

```


#
<h2><b> Find The Percentage:   </b></h2>

```
N = int(input())
STUDENT_MARKS = {}

for line in range(N):
    info = input().split(" ")
    grades = list(map(float, info[1:]))
    STUDENT_MARKS[info[0]] = sum(grades) / float(len(grades))

print("%.2f" % round(STUDENT_MARKS[input()], 2))

```


#
<h2><b> Lists:   </b></h2>

```
N = int(input())
ARRAY = []

while N != 0:
    A = input().split()

    if len(A) == 3:
        B = int(A[1])
        C = int(A[2])
    elif len(A) == 2:
        B = int(A[1])

    if A[0] == "insert":
        ARRAY.insert(B, C)
    elif A[0] == "print":
        print(ARRAY)
    elif A[0] == "remove":
        ARRAY.remove(B)
    elif A[0] == "append":
        ARRAY.append(B)
    elif A[0] == "sort":
        ARRAY.sort()
    elif A[0] == "pop":
        ARRAY.pop()
    elif A[0] == "reverse":
        ARRAY.reverse()
    N -= 1

```


#
<h2><b>Tuples:  </b></h2>
<h2>Select Language to Pypy3 and Paste 👇</h2>

```
if __name__ == '__main__':
    n = int(input())
    t = tuple(map(int, input().split()))
    print(hash(t))


```


#
<h2><b> Swap Case:   </b></h2>

```
def swap_case(s):
    '''Swaps upper/lower-case letters to lower/upper-case letters'''
    return s.swapcase()

if __name__ == '__main__':
    s = input()
    result = swap_case(s)
    print(result)


```


#
<h2><b> String Split And Join:   </b></h2>

```
def split_and_join(line):
    '''Converts 'space' to '-' '''
    line = line.split(" ")
    line = "-".join(line)
    return line

if __name__ == '__main__':
    line = input()
    result = split_and_join(line)
    print(result)

```


#
<h2><b> What's Your Name:   </b></h2>

```

#
# Complete the 'print_full_name' function below.
#
# The function is expected to return a STRING.
# The function accepts following parameters:
#  1. STRING first
#  2. STRING last
#

def print_full_name(a, b):
    '''Read name and lastname in one specified line'''
    print("Hello %s %s! You just delved into python."%(a, b))

if __name__ == '__main__':
    first_name = input()
    last_name = input()
    print_full_name(first_name, last_name)

```


#
<h2><b>Mutations:    </b></h2>

```
def mutate_string(string, position, character):
    '''Changes a character at a given index'''
    return string[:position] + character + string[position + 1:]

if __name__ == '__main__':
    s = input()
    i, c = input().split()
    s_new = mutate_string(s, int(i), c)
    print(s_new)


```


#
<h2><b>Find A String:    </b></h2>

```
def count_substring(string, sub_st):
    ans=[1 for i in range(len(string)-len(sub_st)+1) if string[i:i+len(sub_st)] == sub_st]
    ans = sum(ans)
    return ans

if __name__ == '__main__':
    string = input().strip()
    sub_string = input().strip()
    
    count = count_substring(string, sub_string)
    print(count)

```


#
<h2><b> String Validators:   </b></h2>

```

if __name__ == '__main__':
    s = input()

    print(any(i.isalnum() for i in s))
    print(any(i.isalpha() for i in s))
    print(any(i.isdigit() for i in s))
    print(any(i.islower() for i in s))
    print(any(i.isupper() for i in s))

```


#
<h2><b>Text Alignments:    </b></h2>

```
THICKNESS = int(input()) #This must be an odd number
c = 'H'

# Top Cone
for i in range(THICKNESS):
    print((c*i).rjust(THICKNESS-1)+c+(c*i).ljust(THICKNESS-1))

# Top Pillars
for i in range(THICKNESS+1):
    print((c*THICKNESS).center(THICKNESS*2)+(c*THICKNESS).center(THICKNESS*6))

# Middle Belt
for i in range((THICKNESS+1)//2):
    print((c*THICKNESS*5).center(THICKNESS*6))    

# Bottom Pillars
for i in range(THICKNESS+1):
    print((c*THICKNESS).center(THICKNESS*2)+(c*THICKNESS).center(THICKNESS*6))    

# Bottom Cone
for i in range(THICKNESS):
    print(((c*(THICKNESS-i-1)).rjust(THICKNESS)+c+(c*(THICKNESS-i-1)).ljust(THICKNESS)).rjust(THICKNESS*6))

```


#
<h2><b>Text Wraps:    </b></h2>

```
import textwrap

def wrap(string, max_width):
    '''Wraps the string into a paragraph of width w'''
    string = [c for c in string]

    for i in range(max_width, len(string) + max_width, max_width+1):
        string.insert(i, '\n')
    return ("").join(string)

    

if __name__ == '__main__':
    string, max_width = input(), int(input())
    result = wrap(string, max_width)
    print(result)


```


#
<h2><b>Designer Door Mat:    </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

N, M = map(int, input().split())

for i in range(int(N/2)):
    string = ".|." * (2 * i + 1)
    x = string.center(M, '-')
    print(x)

print("WELCOME".center(M, '-'))

for i in reversed(range(int(N/2))):
    string = ".|." * (2 * i + 1)
    x = string.center(M, '-')
    print(x)


```


#
<h2><b> String Fomartting:   </b></h2>

```
def print_formatted(number):
    # your code goes here
    '''Prints number in decinmal, ocal, hexadecimal, and binary'''
    for i in range(1, number + 1):
        width = len(f"{number:b}")
        print(f"{i:{width}} {i:{width}o} {i:{width}X} {i:{width}b}")


if __name__ == '__main__':
    n = int(input())
    print_formatted(n)

```


#
<h2><b> Alphabet Rangoli:   </b></h2>

```
def print_rangoli(size):
    # your code goes here
    '''Prints Rangoli Design'''
    width = size*4-3
    string = ''

    for i in range(1, size+1):
        for j in range(0, i):
            string += chr(96+size-j)
            if len(string) < width:
                string += '-'
        for k in range(i-1, 0, -1):
            string += chr(97+size-k)
            if len(string) < width:
                string += '-'
        print(string.center(width, '-'))
        string = ''

    for i in range(size-1, 0, -1):
        string = ''
        for j in range(0, i):
            string += chr(96+size-j)
            if len(string) < width:
                string += '-'
        for k in range(i-1, 0, -1):
            string += chr(97+size-k)
            if len(string) < width:
                string += '-'
        print(string.center(width, '-'))
if __name__ == '__main__':
    n = int(input())
    print_rangoli(n)


```


#
<h2><b> Capitalize:   </b></h2>

```
#!/bin/python3

import math
import os
import random
import re
import sys
import os
# Complete the solve function below.
def solve(s):
    '''Calculates the capitalized string'''
    s = s.split(" ")
    return " ".join(i.capitalize() for i in s)

if __name__ == '__main__':
    fptr = open(os.environ['OUTPUT_PATH'], 'w')

    s = input()

    result = solve(s)

    fptr.write(result + '\n')

    fptr.close()

```


#
<h2><b>The Minion Game:    </b></h2>

```
def minion_game(string):
    # your code goes here
    '''Calculates name of Winner and their score'''
    stuart = 0
    kevin = 0
    strlen = len(string)

    for i in range(strlen):
        for vowc in "AEIOU":
            if string[i].find(vowc) >= 0:
                kevin = kevin + strlen - i

    stuart = int(strlen*(strlen+1)/2) - kevin

    if stuart > kevin:
        print("Stuart " + str(stuart))
    if kevin > stuart:
        print("Kevin " + str(kevin))
    if kevin == stuart:
        print("Draw")

    return 0
if __name__ == '__main__':
    s = input()
    minion_game(s)


```


#
<h2><b> Merge The Tools:   </b></h2>

```
def merge_the_tools(string, k):
    # your code goes here
    x = [string[i:i+k] for i in range(0, len(string), k)]

    for i in x:
        j = 0
        short = ""
        for _ in i:
            if i.index(_) == j:
                short += _
            j += 1
        print(short)

if __name__ == '__main__':
    string, k = input(), int(input())
    merge_the_tools(string, k)

```


#
<h2><b>itertools.product():    </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

from itertools import product

A = list(map(int,input().strip().split()))
B = list(map(int,input().strip().split()))

ans = [str(i) for i in list(product(A,B))]
print (' '.join(ans))

```


#
<h2><b> collections.Counter():   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

X = int(input())
shoe_sizes = list(map(int,input().strip().split()))

N = int(input())

earned_amount = []
for n in range(N):
    desired_size,price = list(map(int,input().strip().split()))
    if desired_size in shoe_sizes:
        earned_amount.append(price)
        shoe_sizes.remove(desired_size)

print (sum(earned_amount))

```


#
<h2><b>itertools.permutations():    </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

import itertools

strg,k = input().strip().split()
strg = ''.join(sorted(strg))
perms = list(itertools.permutations(strg,int(k)))
for p in perms:
    print (''.join(p))


```


#
<h2><b>Polar Coordinates:    </b></h2>

```

# Enter your code here. Read input from STDIN. Print output to STDOUT

import cmath
complex_num = complex(input())

print (abs(complex_num))
print (cmath.phase(complex_num))

```


#
<h2><b> Introduction To Sets:   </b></h2>

```
def average(array):
    # your code goes here
    '''Calculates the average of the array'''
    s = set(arr)
    return float(sum(s)) / len(s)
if __name__ == '__main__':
    n = int(input())
    arr = list(map(int, input().split()))
    result = average(arr)
    print(result)


```


#
<h2><b> DefaultDict Tutorial:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


from collections import defaultdict

N, M = map(int, input().split())
D = defaultdict(list)

for i in range(1, N + 1):
    D[input()].append(str(i))
for i in range(M):
    print(' '.join(D[input()]) or -1)

```


#
<h2><b> Calendar Module:
   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

import calendar

MONTH, DAY, YEAR = map(int, input().split())

print(calendar.day_name[calendar.weekday(YEAR, MONTH, DAY)].upper())



```


#
<h2><b> Exceptions:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


for _ in range(int(input())):
    try:
        a, b = input().split()
        print(int(a) // int(b))
    except ZeroDivisionError as z:
        print(f'Error Code: {z}')
    except ValueError as v:
        print(f'Error Code: {v}')

```


#
<h2><b>Collections.namedtuple():    </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


from collections import namedtuple

N, STUDENT = int(input()), namedtuple('Student', input())

print("{:.2f}".format(sum([int(STUDENT(*input().split()).MARKS) for _ in range(N)]) / N))



```


#
<h2><b>Time Delta:    </b></h2>

```
from datetime import datetime

format = '%a %d %b %Y %H:%M:%S %z'

for _ in range(int(input())):
    time1 = datetime.strptime(input(), format)
    time2 = datetime.strptime(input(), format)

    print(int(abs((time1 - time2).total_seconds())))

```


#
<h2><b>Find Angle MBC:    </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

import math
AB = int(input())
BC = int(input())

if AB == BC:
    print (round(math.degrees(math.asin(1/math.sqrt(2)))),chr(176),sep='')

else:
    x = AB/BC
    print (round(math.degrees(math.atan(x))),chr(176),sep='')


```


#
<h2><b>No Idea:    </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


N = input().split()
M = input().split()
A = set(input().split())
B = set(input().split())

COUNTER = 0

for i in M:
    if i in A:
        COUNTER += 1
    if i in B:
        COUNTER -= 1

print(COUNTER)

```


#
<h2><b>Collections.OrderedDict():    </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


from collections import OrderedDict

A_LIST = OrderedDict()

N = int(input())

for i in range(N):
    inp = input()

    if type(inp) != int:
        isplit = inp.split()
        cost = isplit[-1]
        item = isplit[:-1]
        item = " ".join(item)
        cost = "".join(cost)
        cost = int(cost)

        if item in A_LIST:
            current = A_LIST[item]
            current += cost
            A_LIST[item] = current
        else:
            A_LIST[item] = cost


for key, value in A_LIST.items():
    print(key, value)



```


#
<h2><b> Symmetric Difference:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


m = int(input())

a = set(map(int, input().split()))

n = int(input())

b = set(map(int, input().split()))

# Difference in each sets
c = a.difference(b)
d = b.difference(a)

# Union of difference
e = c.union(d)

# Converting set to a list
RESULT = list(e)

# Sorting
RESULT.sort()

# Iteration
for i in range(len(RESULT)):
    print(RESULT[i])




```


#
<h2><b>    </b></h2>

```


```


#
<h2><b> itertools.combinations():    </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

from itertools import combinations

S, N = input().split()

for i in range(1, int(N)+1):
    for j in combinations(sorted(S), i):
        print(''.join(j))

```


#
<h2><b> Incorrect Regex:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


import re

for _ in range(int(input())):
    try:
        a = re.compile(input())
        print("True")
    except Exception:
        print("False")

```


#
<h2><b>Sets.add():    </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


n = int(input())

NAMES = set([])

for i in range(n):
    NAMES.add(input())

print(len(NAMES))

```


#
<h2><b> itertools.combinations_with_replacement():   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


from itertools import combinations_with_replacement

S, k = map(str, input().split())

S = sorted(S)
k = int(k)

for e in list(combinations_with_replacement(S, k)):
    print(*e, sep='')


```


#
<h2><b> Word Order:    </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


from collections import Counter

N = int(input())
LIST = []

for i in range(N):
    LIST.append(input().strip())

COUNT = Counter(LIST)

print(len(COUNT))
print(*COUNT.values())




```


#
<h2><b> Set .discard(), .remove() & .pop():   </b></h2>

```
n = int(input())
s = set(map(int, input().split()))


for i in range(int(input())): # Iterate in range of the input num
    s1 = input().split()
    if s1[0] == 'pop':
        s.pop()
    elif s1[0] == 'remove':
        s.remove(int(s1[1]))
    elif s1[0] == 'discard':
        s.discard(int(s1[1]))

print(sum(s))

```


#
<h2><b> Collections.deque():   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


from collections import deque

D = deque()

for _ in range(int(input())):
    oper, val, *args = input().split() + ['']
    eval(f'D.{oper} ({val})')

print(*D)

```


#
<h2><b> Compress the String! :   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


from itertools import groupby

for k, c in groupby(input()):
    print("(%d, %d)" % (len(list(c)), int(k)), end=' ')


```


#
<h2><b> Company Logo:   </b></h2>

```

1)

def companyLogo(s):
    literal_cnts = {}
    dist_letters = set(s)
    for char in dist_letters:
        literal_cnts[char] = s.count(char)
    sorted_kv = sorted(literal_cnts.items(),key=lambda x: (x[1],-ord(x[0])),reverse=True)
    top_3 = sorted_kv[:3]
    if top_3[0][1] == top_3[1][1] and top_3[0][1] > top_3[2][1]:
        top_3[:2] = sorted(top_3[:2])
    elif top_3[1][1] == top_3[2][1]:
        top_3[1:] = sorted(top_3[1:])
    elif top_3[0][1] == top_3[1][1] == top_3[2][1]:
        top_3 = sorted(top_3)
    for k,v in top_3:
        print (k,v)
        
if __name__ == '__main__':
    
    S = input()
    companyLogo(S)


2)

from collections import Counter

S = input()
S = sorted(S)

FREQUENCY = Counter(list(S))

for k, v in FREQUENCY.most_common(3):
    print(k, v)

```


#
<h2><b>Set .union() Operation:    </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


_ = int(input())
SET_N = set(map(int, input().split()))

_ = int(input())
SET_B = set(map(int, input().split()))

NEW_SET = SET_N.union(SET_B)
print(len(NEW_SET))

```


#
<h2><b> Pilling Up:    </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


T = int(input())
for t in range(T):
    N = int(input())
    lst = list(map(int, input().strip().split()))
    L = len(lst)
    i = 0
    while i < L - 1 and lst[i] >= lst[i+1]:
        i += 1
    while i < L - 1 and lst[i] <= lst[i+1]:
        i += 1
    print ("Yes" if i == L - 1 else "No")



```


#
<h2><b>Triangle Quest 2:    </b></h2>

```

for i in range(1,int(input())+1): #More than 2 lines will result in 0 score.
    print (((10**i-1)//9)**2)


```


#
<h2><b> Iterables and Iterators:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


from itertools import combinations

N = int(input())
LETTERS = list(input().split(" "))
K = int(input())

TUPLES = list(combinations(LETTERS, K))
CONTAINS = [word for word in TUPLES if "a" in word]

print(len(CONTAINS)/len(TUPLES))


```


#
<h2><b> Set .intersection() Operation:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

_ = int(input())
SET_N = set(map(int, input().split()))

_ = int(input())
SET_B = set(map(int, input().split()))

print(len(SET_N & SET_B))

```


#
<h2><b> Mod Divmod:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

A = int(input())
B = int(input())

print(A//B)
print(A%B)
print(divmod(A, B))

```


#
<h2><b> Power - Mod Power:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

import math

a = int(input())
b = int(input())
m = int(input())

c = math.pow(a, b)
d = c%m

print(int(c))
print(int(d))

```


#
<h2><b> Maximize It!:    </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT
import itertools

NUMBER_OF_LISTS, MODULUS = map(int, input().split())
LISTS_OF_LISTS = []

for i in range(0, NUMBER_OF_LISTS):
    new_list = list(map(int, input().split()))
    del new_list[0]
    LISTS_OF_LISTS.append(new_list)

def squared(element):
    return element**2

COMBS = list(itertools.product(*LISTS_OF_LISTS))
RESULTS = []

for i in COMBS:
    result1 = sum(map(squared, [a for a in i]))
    result2 = result1 % MODULUS
    RESULTS.append(result2)

print(max(RESULTS))

```


#
<h2><b> Set .difference() Operation:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

_ = int(input())
SET_N = set(map(int, input().split()))

_ = int(input())
SET_B = set(map(int, input().split()))

NEW_SET = SET_N.difference(SET_B)
print(len(NEW_SET))

```


#
<h2><b> Integers Come In All Sizes:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

a = int(input())
b = int(input())
c = int(input())
d = int(input())

print((a**b)+(c**d))

```


#
<h2><b>Set .symmetric_difference() Operation:    </b></h2>

```

# Enter your code here. Read input from STDIN. Print output to STDOUT


_ = int(input())
SET_N = set(map(int, input().split()))

_ = int(input())
SET_B = set(map(int, input().split()))

print(len(SET_N.symmetric_difference(SET_B)))

```


#
<h2><b> Set Mutations:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

A = int(input())
SET_A = set(map(int, input().split()))
N = int(input())

for _ in range(N):
    operation = input().split()
    new_set = set(map(int, input().split()))
    eval('SET_A.{}({})'.format(operation[0], new_set))

print(sum(SET_A))


```


#
<h2><b> Triangle Quest:   </b></h2>

```
for i in range(1,int(input())): #More than 2 lines will result in 0 score. Do not leave a blank line also
    print((10**(i)//9)*i)

```


#
<h2><b> The Captain's Room:    </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


k = int(input())

arr = list(map(int, input().split()))

my_set = set(arr)

print(((sum(my_set)*k)-(sum(arr)))//(k-1))

```


#
<h2><b>Check Subset:    </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


for i in range(int(input())):
    a = int(input())
    set_a = set(map(int, input().split()))

    b = int(input())
    set_b = set(map(int, input().split()))

    if len(set_a - set_b) == 0:
        print("True")
    else:
        print("False")



```


#
<h2><b> Check Strict Superset:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

A = set(input().split())
COUNT = 0
VALUE = 0

for i in range(int(input())):
    if A.issuperset(set(input().split())):
        COUNT += 1
    else:
        VALUE += 1
if VALUE != 0:
    print('False')
else:
    print('True')

```


#
<h2><b> Classes: Dealing with Complex Numbers:   </b></h2>

```
import math


class Complex(object):
    def __init__(self, real, imaginary):
        self.real = real
        self.imaginary = imaginary

    def __add__(self, no):
        return Complex((self.real+no.real), self.imaginary+no.imaginary)

    def __sub__(self, no):
        return Complex((self.real-no.real), (self.imaginary-no.imaginary))

    def __mul__(self, no):
        r = (self.real*no.real)-(self.imaginary*no.imaginary)
        i = (self.real*no.imaginary+no.real*self.imaginary)
        return Complex(r, i)

    def __truediv__(self, no):
        conjugate = Complex(no.real, (-no.imaginary))
        num = self*conjugate
        denom = no*conjugate
        try:
            return Complex((num.real/denom.real), (num.imaginary/denom.real))
        except Exception as e:
            print(e)

    def mod(self):
        m = math.sqrt(self.real**2+self.imaginary**2)
        return Complex(m, 0)

    def __str__(self):
        if self.imaginary == 0:
            result = "%.2f+0.00i" % (self.real)
        elif self.real == 0:
            if self.imaginary >= 0:
                result = "0.00+%.2fi" % (self.imaginary)
            else:
                result = "0.00-%.2fi" % (abs(self.imaginary))
        elif self.imaginary > 0:
            result = "%.2f+%.2fi" % (self.real, self.imaginary)
        else:
            result = "%.2f-%.2fi" % (self.real, abs(self.imaginary))
        return result
if __name__ == '__main__':
    c = map(float, input().split())
    d = map(float, input().split())
    x = Complex(*c)
    y = Complex(*d)
    print(*map(str, [x+y, x-y, x*y, x/y, x.mod(), y.mod()]), sep='\n')

```


#
<h2><b> Class 2 - Find the Torsional Angle:   </b></h2>

```
import math

class Points(object):
    def __init__(self, x, y, z):
        self.x = x
        self.y = y
        self.z = z

    def __sub__(self, no):
        return  Points((self.x-no.x), (self.y-no.y), (self.z-no.z))

    def dot(self, no):
        return (self.x*no.x)+(self.y*no.y)+(self.z*no.z)

    def cross(self, no):
        return Points((self.y*no.z-self.z*no.y), (self.z*no.x-self.x*no.z), (self.x*no.y-self.y*no.x))

    def absolute(self):
        return pow((self.x ** 2 + self.y ** 2 + self.z ** 2), 0.5)
if __name__ == '__main__':
    points = list()
    for i in range(4):
        a = list(map(float, input().split()))
        points.append(a)

    a, b, c, d = Points(*points[0]), Points(*points[1]), Points(*points[2]), Points(*points[3])
    x = (b - a).cross(c - b)
    y = (c - b).cross(d - c)
    angle = math.acos(x.dot(y) / (x.absolute() * y.absolute()))

    print("%.2f" % math.degrees(angle))


```


#
<h2><b> Zipped!:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

#!/usr/bin/env python3

if __name__ == "__main__":
    st_num, sb_num = map(int, input().strip().split())
    scores = []
    
    for _ in range(sb_num):
        scores.append(map(float, input().strip().split()))
        
    for el in zip(*scores):
        print(sum(el)/sb_num)

```


#
<h2><b> Input():   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

if __name__ == "__main__":
    x, k = map(int, input().strip().split())
    string = input().strip()
    
    if eval(string) == k:
        print(True)
    else:
        print(False)

```


#
<h2><b> Python Evaluation:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

#!/usr/bin/env python3

if __name__ == "__main__":
    eval(input().strip())

```


#
<h2><b> Athlete Short:   </b></h2>

```
1)

#!/bin/python3

import math
import os
import random
import re
import sys



if __name__ == '__main__':
    nm = input().split()

    n = int(nm[0])

    m = int(nm[1])

    arr = []

    for _ in range(n):
        arr.append(list(map(int, input().rstrip().split())))

    k = int(input())

    P=sorted(arr,key=lambda row:row[k])
    for i in range(len(P)):
        for j in range(len(P[i])):
            print(P[i][j], end=' ')
        print()


2)

# Enter your code here. Read input from STDIN. Print output to STDOUT
tbl = []
rc = input()
(r,c) = map(int, rc.split())

for i in range(r):
    _row = input()
    row = list(map(int, _row.split()))
    tbl.append(row)

idx = int(input())
    
tbls = sorted(tbl, key = lambda x: x[idx])
for t in tbls:
    print (*t)



```


#
<h2><b> Any or all:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

#!/usr/bin/env python3

if __name__ == "__main__":
    num_cnt = int(input().strip())
    arr = list(input().strip().split())
    print(all([all([int(x) > 0 for x in arr]), any([x == x[::-1] for x in arr])]))
        


```


#
<h2><b> ginortS:   </b></h2>

```

#!/usr/bin/env python3

if __name__ == "__main__":
    string = input().strip()
    
    print(*sorted(string, key = lambda x: (-x.islower(), x.isdigit() - x.isupper(), x in '02468', x)), sep='')



```


#
<h2><b> Detect Floating Point Number: </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


from re import match, compile

pattern = compile('^[-+]?\d*\.\d+$')
for _ in range(int(input())):
    print(bool(pattern.match(input())))

```


#
<h2><b> Map and Lambda Function:    </b></h2>

```
cube = lambda x: x**3 

def fibonacci(n):
    # return a list of fibonacci numbers
    if n == 0:
        return []
    if n == 1:
        return [0]
    prev = 0
    cur = 1
    out = [prev, cur]
    
    for _ in range(n-2):
        prev, cur = cur, prev + cur
        out.append(cur)
        
    return out


if __name__ == '__main__':
    n = int(input())
    print(list(map(cube, fibonacci(n))))


```


#
<h2><b> Re.split():   </b></h2>

```
regex_pattern = r'[.,]+'	# Do not delete 'r'.
import re
print("\n".join(re.split(regex_pattern, input())))

```


#
<h2><b> Validating Email Addresses With a Filter:    </b></h2>

```
import re
def fun(s):
    # return True if s is a valid email, else return False
    '''
    n=int(input())
    e=[]
    for _ in range[n]:
        e.append(input())
    user= e.split("@")[0]
    print(user)
    '''
    '''
    l = list(map(lambda x:x.split("@")[0], s))
    l = list(filter(lambda x: x > 10 and x < 80, l))
    '''
    #print(s)
    ptrn = re.compile("^[a-zA-Z][\w-]*@[a-zA-Z0-9]+\.[a-zA-Z]{1,3}$")
    result = ptrn.match(s)
    #l = list(filter(lambda x:x.match(ptrn) , s))
    return result
def filter_mail(emails):
    return list(filter(fun, emails))

if __name__ == '__main__':
    n = int(input())
    emails = []
    for _ in range(n):
        emails.append(input())

filtered_emails = filter_mail(emails)
filtered_emails.sort()
print(filtered_emails)


```


#
<h2><b> Group(), Groups() & Groupdict():   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

import re
s = input()
res = re.search(r'([A-Za-z0-9])\1',s)
if res == None:
    print(-1)
else:
    print(res.group(1))

```


#
<h2><b> Reduce Function:    </b></h2>

```
from fractions import Fraction
from functools import reduce

def product(fracs):
    t = reduce(lambda x, y : x * y, fracs) # complete this line with a reduce statement
    return t.numerator, t.denominator

if __name__ == '__main__':
    fracs = []
    for _ in range(int(input())):
        fracs.append(Fraction(*map(int, input().split())))
    result = product(fracs)
    print(*result)

```


#
<h2><b> Re.findall() & Re.finditer():   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

#!/usr/bin/env python3

import re

cons = 'QWRTYPSDFGHJKLZXCVBNMqwrtypsdfghjklzxcvbnm'
vowels = 'AEIOUaeiou'

if __name__ == "__main__":
    string = input().strip()
    
    m = re.findall(r"(?<=[%s])([%s]{2,})[%s]" % (cons, vowels, cons), string)
    
    print("\n".join(m or ['-1']))

```


#
<h2><b> Re.start() & Re.end():   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

#!/usr/bin/env python3

import re

if __name__ == "__main__":
    string = input()
    sub = input()
    
    matches = list(re.finditer(r'(?={})'.format(sub), string))
    
    if matches:
        for match in matches:
            print((match.start(), match.end() + len(sub) - 1))
    else:
        print((-1, -1))

```


#
<h2><b> Regex Substitution:    </b></h2>

```

# Enter your code here. Read input from STDIN. Print output to STDOUT

import re, sys
n = int(input())
for line in sys.stdin:
    remove_and = re.sub(r'(?<= )(&&)(?= )',"and",line)
    remove_or = re.sub(r'(?<= )(\|\|)(?= )',"or",remove_and)
    print(remove_or,end='')

```


#
<h2><b> Validating Roman Numerals:   </b></h2>

```
regex_pattern = r"^M{0,3}(CM|CD|D?C{0,3})(XC|XL|L?X{0,3})(IX|IV|V?I{0,3})$"	# Do not delete 'r'.

import re
print(str(bool(re.match(regex_pattern, input()))))

```


#
<h2><b> Validating phone numbers:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


import re

n = int(input().strip())

for _ in range(n):
    tel = input().strip()
    pattern = '^[789][0-9]{9}$'
    print("{}".format("YES" if bool(re.match(pattern, tel)) else "NO"))

```


#
<h2><b> Validating and Parsing Email Addresses:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

import re, email.utils
n = int(input())
for t in range(n):
    s = input()
    parsed_email = email.utils.parseaddr(s)[1].strip()
    match_result = bool(re.match(r'(^[A-Za-z][A-Za-z0-9\._-]+)@([A-Za-z]+)\.([A-Za-z]{1,3})$',parsed_email))
    if match_result == True:
        print(s)

```


#
<h2><b> Hex Color Code:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

import re

n = int(input().strip())
inside = False
for _ in range(n):
    line = input()
    
    for el in line.split(' '):
        if el == "{":
            inside = True
            continue
        elif el == "}":
            inside = False
            continue
        elif inside:
            found = re.search(r'\#[0-9a-fA-F]{3,6}', el)
            if found:
                print(found.group(0))


```


#
<h2><b> HTML Parser - Part 1:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT

import re
from html.parser import HTMLParser

class MyHTMLParser(HTMLParser):
    def handle_starttag(self, tag, attrs):
        print("Start".ljust(6) + ":", tag)
        for at in attrs:
            print("-> {} > {}".format(at[0], at[1]))
    def handle_endtag(self, tag):
        print("End".ljust(6) + ":", tag)
    def handle_startendtag(self, tag, attrs):
        print("Empty".ljust(6) + ":", tag)
        for at in attrs:
            print("-> {} > {}".format(at[0], at[1]))

if __name__ == "__main__":
    parser = MyHTMLParser()
    n = int(input().strip())
    for _ in range(n):
        line = input()
        parser.feed(line)

```


#
<h2><b> HTML Parser -Part 2:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


from html.parser import HTMLParser

class MyHTMLParser(HTMLParser):
    def handle_comment(self, data):
        if data.count('\n') > 0:
            print(">>> Multi-line Comment")
        else:
            print(">>> Single-line Comment")
        print(data)
    def handle_data(self, data):
        if len(data) > 1:
            print(">>> Data")
            print(data)

html = ""       
for i in range(int(input())):
    html += input().rstrip()
    html += '\n'
    
parser = MyHTMLParser()
parser.feed(html)
parser.close()

```


#
<h2><b> Detect HTML Tags, Attributes and Attribute Values:    </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


from html.parser import HTMLParser

class MyHTMLParser(HTMLParser):
    def handle_starttag(self, tag, attrs):
        print(tag)
        for at in attrs:
            print("-> {} > {}".format(at[0], at[1]))
    def handle_startendtag(self, tag, attrs):
        print(tag)
        for at in attrs:
            print("-> {} > {}".format(at[0], at[1]))

html = ""
for i in range(int(input())):
    html += input().rstrip()
    html += '\n'
    
parser = MyHTMLParser()
parser.feed(html)
parser.close()

```


#
<h2><b> XML 1 - Find the Score:   </b></h2>

```

import sys
import xml.etree.ElementTree as etree

def get_attr_number(node):
    # your code goes here
    return len(node.attrib) + sum([get_attr_number(child) for child in node])

if __name__ == '__main__':
    sys.stdin.readline()
    xml = sys.stdin.read()
    tree = etree.ElementTree(etree.fromstring(xml))
    root = tree.getroot()
    print(get_attr_number(root))

```


#
<h2><b> Validating UID:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT



import re

if __name__ == "__main__":
    t = int(input().strip())
    
    for _ in range(t):
        uid = "".join(sorted(input()))
        if (len(uid) == 10 and
            re.match(r'', uid) and 
            re.search(r'[A-Z]{2}', uid) and
            re.search(r'\d\d\d', uid) and
            not re.search(r'[^a-zA-Z0-9]', uid) and
            not re.search(r'(.)\1', uid)):
            print("Valid")
        else:
            print("Invalid")


```


#
<h2><b> Validating Credit Card Numbers:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT


import re

if __name__ == "__main__":
    t = int(input().strip())
    
    for _ in range(t):
        num = "".join(input())
        if (re.match(r'^[456]', num) and
            (re.match(r'([\d]{4}-){3}[\d]{4}$', num) or
             re.match(r'[\d]{16}', num)) and
            not re.search(r'(\d)\1{3,}', num.replace("-", ""))):
            print("Valid")
        else:
            print("Invalid")



```


#
<h2><b> XML2 - Find the Maximum Depth:   </b></h2>

```
import xml.etree.ElementTree as etree

maxdepth = 0
def depth(elem, level):
    global maxdepth
    # your code goes here
    maxdepth = 0
def depth(elem, level):
    #print(elem)
    if level == -1:
        level = 0
    global maxdepth
    if level > maxdepth:
        maxdepth = level
    for el in elem:
        depth(el, level+1)
if __name__ == '__main__':
    n = int(input())
    xml = ""
    for i in range(n):
        xml =  xml + input() + "\n"
    tree = etree.ElementTree(etree.fromstring(xml))
    depth(tree.getroot(), -1)
    print(maxdepth)

```


#
<h2><b> Standardize Mobile Number Using Decorators:   </b></h2>

```
def wrapper(f):
    def fun(l):
        # complete the function
        out = []
        for telnum in l:
            barenum = telnum[-10:]
            telnum = '+91 ' + barenum[:5] + ' ' + barenum[5:]
            out.append(telnum)
        f(out)
    return fun

@wrapper
def sort_phone(l):
    print(*sorted(l), sep='\n')

if __name__ == '__main__':
    l = [input() for _ in range(int(input()))]
    sort_phone(l) 

```


#
<h2><b> Validating Postal Codes:   </b></h2>

```

regex_integer_in_range = r'^[1-9][\d]{5}$'	# Do not delete 'r'.
regex_alternating_repetitive_digit_pair = r'(\d)(?=\d\1)'	# Do not delete 'r'.


import re
P = input()

print (bool(re.match(regex_integer_in_range, P)) 
and len(re.findall(regex_alternating_repetitive_digit_pair, P)) < 2)

```


#
<h2><b> Decorators 2 - Name Directory:   </b></h2>

```
import operator
def person_lister(func):
    def inner(people):
        return [func(p) for p in sorted(people, key = lambda x: (int(x[2])))]
    return inner

@person_lister
def name_format(person):
    return ("Mr. " if person[3] == "M" else "Ms. ") + person[0] + " " + person[1]

if __name__ == '__main__':
    people = [input().split() for i in range(int(input()))]
    print(*name_format(people), sep='\n')

```


#
<h2><b> Matrix Script:   </b></h2>

```
import re

n, m = input().strip().split(' ')
n, m = [int(n), int(m)]
matrix = []
for _ in range(n):
    matrix_t = str(input())
    matrix.append(matrix_t)
    
complete = ""
for el in zip(*matrix):
    complete += "".join(el)
print(re.sub(r'(?<=\w)([^\w]+)(?=\w)', " ", complete))

```


#
<h2><b> Words Score:   </b></h2>

```
def is_vowel(letter):
    return letter in ['a', 'e', 'i', 'o', 'u', 'y']

def score_words(words):
    score = 0
    for word in words:
        num_vowels = 0
        for letter in word:
            if is_vowel(letter):
                num_vowels += 1
        if num_vowels % 2 == 0:
            score += 2
        else:
            score += 1
            
    return score


n = int(input())
words = input().split()
print(score_words(words))

```


#
<h2><b>Arrays:    </b></h2>

```
import numpy

def arrays(arr):
    # complete this function
    # use numpy.array
    return(numpy.array(arr[::-1], float))

arr = input().strip().split(' ')
result = arrays(arr)
print(result)

```


#
<h2><b> Shape and Reshape:   </b></h2>

```
# Enter your code here. Read input from STDIN. Print output to STDOUT
import numpy
ar = list(map(int,input().split()))
np_ar = numpy.array(ar)
print(numpy.reshape(np_ar,(3,3)))

```


#
<h2><b> Default Arguments:   </b></h2>

```
class EvenStream(object):
    def __init__(self):
        self.current = 0

    def get_next(self):
        to_return = self.current
        self.current += 2
        return to_return

class OddStream(object):
    def __init__(self):
        self.current = 1

    def get_next(self):
        to_return = self.current
        self.current += 2
        return to_return

def print_from_stream(n, stream=EvenStream()):
    stream.__init__()
    for _ in range(n):
        print(stream.get_next())


queries = int(input())
for _ in range(queries):
    stream_name, n = input().split()
    n = int(n)
    if stream_name == "even":
        print_from_stream(n)
    else:
        print_from_stream(n, OddStream())


```


#
<h2><b> Transpose and Flatten:   </b></h2>

```
import numpy
n,m = map(int,input().split())
ar = []
for i in range(n):
    row = list(map(int,input().split()))
    ar.append(row)

np_ar = numpy.array(ar)
print(numpy.transpose(np_ar))
print(np_ar.flatten())

```


#
<h2><b> Concatenate:   </b></h2>

```
import numpy

n,m,p=map(int,input().split())

ar1 = []
ar2 = []
for i in range(n):
    tmp = list(map(int,input().split()))
    ar1.append(tmp)
for i in range(m):
    tmp = list(map(int,input().split()))
    ar2.append(tmp)    
np_ar1 = numpy.array(ar1)
np_ar2 = numpy.array(ar2)
print(numpy.concatenate((np_ar1,np_ar2),axis = 0))


```


#
<h2><b> Zeros and Ones:    </b></h2>

```
import numpy



n_ar = list(map(int,input().split()))
n = tuple(n_ar)
print(numpy.zeros(n,dtype=numpy.int))
print(numpy.ones(n,dtype=numpy.int))

```


#
<h2><b> Eye and Identity:   </b></h2>

```
import numpy as np

np.set_printoptions(legacy='1.13')
n, m = map(int, input().split())
print(np.eye(n, m, k=0))

```


#
<h2><b>Array Mathematics:    </b></h2>

```
import numpy

n,m = map(int,input().split())
ar1 = []
ar2 = []
for i in range(n):
    tmp = list(map(int,input().split()))
    ar1.append(tmp)
for i in range(n):
    tmp = list(map(int,input().split()))
    ar2.append(tmp)
np_ar1 = numpy.array(ar1)
np_ar2 = numpy.array(ar2)
print(np_ar1 + np_ar2)
print(np_ar1 - np_ar2)
print(np_ar1 * np_ar2)
print(np_ar1 // np_ar2)
print(np_ar1 % np_ar2)
print(np_ar1 ** np_ar2)

```


#
<h2><b>Floor, Ceil and Rint:    </b></h2>

```

import numpy as np

np.set_printoptions(legacy='1.13')
A = np.array(input().split(), float)
print(np.floor(A))
print(np.ceil(A))
print(np.rint(A))

```


#
<h2><b> Sum and Prod:   </b></h2>

```
import numpy



n,m=map(int,input().split())
ar = []
for i in range(n):
    tmp = list(map(int,input().split()))
    ar.append(tmp)
np_ar = numpy.array(ar)
s = numpy.sum(np_ar,axis=0)
print(numpy.prod(s))

```


#
<h2><b> Min and Max:   </b></h2>

```
import numpy

n,m = map(int,input().split())
ar = []
for i in range(n):
    tmp = list(map(int,input().split()))
    ar.append(tmp)
np_ar = numpy.array(ar)
print(numpy.max(numpy.min(np_ar,axis=1)))

```


#
<h2><b>Mean, Var, and Std:   </b></h2>

```
import numpy
N, M = map(int, input().split())
A = numpy.array([list(map(int, input().split())) for n in range(N)])
print(numpy.mean(A, axis = 1))
print(numpy.var(A, axis = 0))
print(numpy.round(numpy.std(A), 11))

```


#
<h2><b> Dot and Cross:   </b></h2>

```
import numpy
n = int(input())
ar1 = []
ar2 = []
for i in range(n):
    tmp = list(map(int,input().split()))
    ar1.append(tmp)
np_ar1 = numpy.array(ar1)
for i in range(n):
    tmp = list(map(int,input().split()))
    ar2.append(tmp)
np_ar2 = numpy.array(ar2)
print(numpy.dot(np_ar1,np_ar2))

```


#
<h2><b> Inner and Outer:    </b></h2>

```
import numpy



np_ar1 = numpy.array(list(map(int,input().split())))
np_ar2 = numpy.array(list(map(int,input().split())))
print(numpy.inner(np_ar1,np_ar2))
print(numpy.outer(np_ar1,np_ar2))

```


#
<h2><b> Polynomials:   </b></h2>

```
import numpy as np

l = list(map(float, input().split()))
x=int(input())
arr=np.array(l)
print(np. polyval(arr,x))

```


#
<h2><b> Linear Algebra:   </b></h2>

```
import numpy as np


np.set_printoptions(legacy='1.13')
n = int(input())
array = np.array([input().split() for _ in range(n)], float)
print(np.linalg.det(array))

```

