# Python Program

**1. Getting input for array**         
```py
from array import *
inp=input().split()
vals=([int(a) for a in inp])
print(vals)
```
**Input :**
```input
1 2 3 4 5
```
**Output :**
```csharp
[1, 2, 3, 4, 5]
```

**2. Finding vowel or consonant:**
```python
inp=input("")
if(inp.isalpha()):
    if(inp=='a'or inp=='e'or inp=='i'or inp=='o' or inp=='u'):
        print("vowel")
    else:
        print("consonant")
```
**Input :**
```input
a

```
**Output :**
```csharp
vowel
```

**3. String reverse**
```python
inp=input("")
print(inp[::-1])
```
**Input :**
```input
hello
```
**Output :**
```csharp
olleh
```

**4. Finding string length**
```py
inp=input("")
count=0
for i in inp:
    count=count+1
print(count)
    (OR)
inp = input("")
print(len(inp))
```
**Input :**
```input
string
```
**Output :**
```csharp
6
```

**5. Lower to upper and vice versa**
```py
inp=input("")
count=0
new=inp.swapcase()
print(new)
```
**Input :**
```input
Hello World

```
**Output :**
```csharp
hELLO wORLD

```

**6. Counting number of vowels:**
```py
inp=input("")
count=0
for i in range(len(inp)):
    if(inp[i] in 'aeiou' or inp[i] in 'AEIOU'):
        count=count+1
print(count)
```
**Input :**
```input
education

```
**Output :**
```csharp
5
```

**7. Removing vowels**
```py

inp=input("")
count=0
for i in range(len(inp)):
    if(inp[i] not in 'aeiouAEIOU'):
        print(inp[i],end="")
```
**Input :**
```input
hello world

```
**Output :**
```csharp
hll wrld

```

**8. Finding palindrome of a string**
```py
inp=input("")
count=0
original =inp
reverse=inp[::-1]
for i in range(len(inp)):
    if(original[i]==reverse[i]):
        count=count+1
if(count==len(inp)):
    print("palindrome")
else:
    print("not palindrome")
```
**Input :**
```input
madam
```
**Output :**
```csharp
palindrome
```

**9. Counting space**
```py
inp=input("")
count=0
for i in range(len(inp)):
    if(inp[i].isspace()):
        count =count+1
print(count)
```
**Input :**
```input
hello world python

```
**Output :**
```csharp
2
```

**10. Printing only alphabets**
```py
np=input("")
count=0
for i in range(len(inp)):
    if(inp[i].isalpha()):
        print(inp[i],end="")

```
**Input :**
```input
hello123 world!

```
**Output :**
```csharp
helloworld
```

**11. Removing spaces**
```py
inp=input("")
count=0
for i in range(len(inp)):
    if(inp[i] not in ' '):
        print(inp[i],end="")
```
**Input :**
```input
hello world

```
**Output :**
```csharp
helloworld

```

**12. Counting symbols**
```py
inp=input("")
count=0
for i in range(len(inp)):
    if not inp[i].isalpha() and not inp[i].isdigit():
        count=count+1;
print(count)
```
**Input :**
```input
hello@world#123!

```
**Output :**
```csharp
3
```

**13. Removing brackets**
```py
inp=input("")
count=0
for i in range(len(inp)):
    if(inp[i] not in ')(':
        print(inp[i],end="")
```
**Input :**
```input
(hello) (world)

```
**Output :**
```csharp
hello world

```

**14. Sum of numbers in a string**
```py
inp=input("")
count=0
for i in range(len(inp)):
    if(inp[i].isdigit()):
        count=count+int(inp[i])
print(count)
```
**Input :**
```input
a1b2c3

```
**Output :**
```csharp
6

```

**15. Capitalize first letter of a word:**
```py
inp=input("").split()
count=0
for i in range(len(inp)):
    print(inp[i].capitalize(),end="  ")
```
**Input :**
```input
hello world python

```
**Output :**
```csharp
Hello  World  Python  

```

**16. Printing non repeating characters:**
```py
inp=input("")
for i in range(len(inp)):
      if(inp[i].isalpha()):
          count =0
          for j in range(len(inp)):
              if(inp[i]==inp[j]):
                  count=count+1
      if(count==1):
            print(inp[i],end="")
```
**Input :**
```input
hello

```
**Output :**
```csharp
heo

```

**17. Removing duplicates:**
```py
inp=input("")
result=""
for i in inp:
    if i not in result:
        result+=iand 
print(result)
```
**Input :**
```input
hello

```
**Output :**
```csharp
helo

```

**18. For findng frequency:**
```py
inp=input()
result=""
for i in  range(len(inp)):
    if inp[i] not in result:
        result+=inp[i]
        a=inp.count(inp[i])
        print("%c - %d" % (inp[i], a))
```
**Input :**
```input
hello

```
**Output :**
```csharp
h - 1
e - 1
l - 2
o - 1

```

**19. Separating odd and even:**
```py
numbers=tuple(map(int,input("").split(" ")))
tup1=()
tup2=()
lis1=[]
lis2=[]
a=0
b=0
lis=list(numbers)
for i in lis:
    if (i%2==0):
        lis1.append(i)
    else:
        lis2.append(i)
tup1=tuple(lis1)
tup2=tuple(lis2)
print(tup1)
print(tup2)
```
**Input :**
```input
1 2 3 4 5
```
**Output :**
```csharp
(2, 4)
(1, 3, 5)

```

**20. Removing reoccurring character:**
```py
inp=input("")
result=inp[0]
count=0
for i in range(1,len(inp)):
    if (inp[i]!=inp[i-1]):
        result+=inp[i]
    else:
        count=count+1
if(count!=0):
    print(result)
elif(count==0):
    print("no occurance")
```
**Input :**
```input
aabbcc

```
**Output :**
```csharp
abc

```
**21. Printing acronym:**
```py
inp=input("")
result=inp[0]
for i in range(1,len(inp)):
    if inp[i].isspace():
        result+=inp[i+1]
print(result.upper())
 ```
**Input :**
```input
Hello World Python

```
**Output :**
```csharp
HWP

```

**22. Count concecutive repeating characters:**
```py
inp=input("")
result=""
count=1
for i in range(1,len(inp)):
    if(inp[i]==inp[i-1]):
        count=count+1
    else:
        result+=inp[i-1]+str(count)
        count=1
result+=(inp[-1])+str(count)
print(result)
```
**Input :**
```input
aaabbc

```
**Output :**
```csharp
a3b2c1

```

**23. First non repeating character:**
```py
inp=input("")
for i in range(len(inp)):
    count=0
    for j in range(len(inp)):
        if i==j:
            continue
        if(inp[i]==inp[j]):
            count=count+1
    if(count==0):
        print(inp[i])
        break
```
**Input :**
```input
hello

```
**Output :**
```csharp
h

```

**24. Separating numbers from string and find largest and second largest numbers:**
```py
inp=input("")
result=""
new=""
for i in inp:
    if i.isdigit():
        result+=i
for i in result:
    if i not in new:
        new+=i
a=sorted(new)
b=len(new)
print("first lar %c second lar %c"% (a[b-1],a[b-2]))
```
**Input :**
```input
a3b9c5d1

```
**Output :**
```csharp
first lar 9 second lar 5

```

**25. True if first string is in the second one:**
```Python
inp1=input("")
inp2=input("")
count=0
a=""
for i in range(len(inp1)):
    if inp1[i] not in a:
        a+=inp1[i]
        for j in range(len(inp2)):
            if inp1[i]==inp2[j]:
                count=count+1
print(count)
if(count==len(inp1)):
    print("true")
else:
    print("false")
```
**Input :**
```input
abc
abcdef

```
**Output :**
```arduino
true

```

**26. Replacing word:**
```Python
inp1=input("").split(" ")
inp2=input("")
result=""
for i in inp1:
    if i!=inp2:
        result+=i+" "
print(result)
```
**Input :**
```input
hello world python
world

```
**Output :**
```csharp
hello python

```

**27. Reversing a string:**
```Python
inp1=input("").split(" ")
inp2=inp1[::-1]
for i in inp2:
    print(i,end=" ")
```
**Input :**
```input
hello world python

```
**Output :**
```csharp
python world hello

```

**28. Printing longest words first:**
```Python
inp=input("").split(" ")
inp= sorted(inp,key=len,reverse='true')
print(" ".join(inp))
```
**Input :**
```input
I love programming

```
**Output :**
```csharp
programming love I

```

**29. Printing numbers:**
```Python
inp=input("")
dic={
    'one':'1',
    'two':'2',
    'three':'3',
    'four':'4',
    'five':'5',
    'six':'6',
    'seven':'7',
    'eight':'8',
    'nine':'9'
}
a=''.join(dic[ele] for ele in inp.split(" "))
print(a)
```
**Input :**
```input
one two three

```
**Output :**
```csharp
123

```

**30. Printing index of the word:**
```Python
inp=input("")
w=input("")
a=inp.split(" ")
i=1
for i in range(1,(len(a)+1)):
    if a[i]==w:
        print(i+1)
        break
```
**Input :**
```input
hello world python
world

```
**Output :**
```csharp
2

```

**31. Convert tuple into a string:**
```Python
inp=tuple(map(str,input("").split(" ")))
st="".join(inp)
print(st)
```
**Input :**
```input
hello world

```
**Output :**
```csharp
helloworld

```

**32. Joining characters of list to convert as string**
```Python
a = ['P', 'y', 't', 'h', 'o', 'n']

# Convert list of characters to string
s = ''.join(a)

print(s)
```
**Output :**
```csharp
Python

```

**33. Printing goo pair or not:**
```Python
inp=input("")
a=inp.count(inp[0])
count=0
for i in range(1,len(inp)):
    if(inp.count(inp[i])!=a):
        count=count+1
if(count==0):
    print("good pair")
else:
    print("bad pair")
```
**Input :**
```input
aabb

```
**Output :**
```csharp
good pair

```

**34. Merging two list and sort and then sorting:**
```Python
lis1=tuple(map(int,input("").split(" ")))
lis2=tuple(map(int,input("").split(" ")))
new=list(lis1+lis2)
a=sorted(new)
print(a)
```
**Input :**
```input
1 3 5
2 4 6

```
**Output :**
```csharp
[1, 2, 3, 4, 5, 6]

```

**35. Changing first reoccurred string:**
```python
inp=input("")
result=""
for i in range(len(inp)):
    if inp[i] not in result:
        result+=inp[i]
    else:
        result+='$'
        break
a=len(inp)
b=len(result)
c=a-b
result+=inp[-c:]
print(result)
```
**Input :**
```input
hello

```
**Output :**
```csharp
hel$o

```

**36. Swapping last two words between two strings:**
```python
inp1=input("")
inp2=input("")
a=len(inp1)-1
b=len(inp2)-1
new1=""
new2=""
for i in range(a):
    new1+=inp1[i]
new1+=inp2[-1:]
for i in range(b):
    new2+=inp2[i]
new2+=inp1[-1:]
print(new1)
print(new2)
```
**Input :**
```input
hello world
python code

```
**Output :**
```csharp
hello code
python world

```

**37. Removing character with index:**
```python
inp=input("")
num=int(input(""))
result=""
for i in range(len(inp)):
    if i==num:
        result+=""
    else:
        result+=inp[i]
print(result)
```
**Input :**
```input
hello
2

```
**Output :**
```csharp
helo

```

**38. Removing odd index character:**
```python
inp=input("")
result=""
for i in range(len(inp)):
    if i%2!=0:
        result+=""
    else:
        result+=inp[i]
print(result)
```
**Input :**
```input
abcdef

```
**Output :**
```csharp
ace

```

**39. Printing most frequemt character:**
```python
inp=input("")
maxi=inp.count(inp[0])
result=""
ch=inp[0]
count=0
for i in range(1,len(inp)):
    if inp[i] not in result:
        if((maxi)<(inp.count(inp[i]))):
            count=count+1
            ch=inp[i]
            maxi=inp.count(inp[i])
            result+=inp[i]
print(ch)
```
**Input :**
```input
hello

```
**Output :**
```csharp
l

```

**40. First non-repeating character:**
```python
inp=input("")
for i in inp:
    a=inp.count(i)
    if a==1:
        print(i)
        break
```
**Input :**
```input
swiss

```
**Output :**
```csharp
w

```

**41. Second most frequent character:**
```python
inp=input("")
result=""
first=""
second=""
for i in inp:
    if i not in result:
        result+=i    
first=max(result,key=inp.count)
result=result.replace(first,"")
second=max(result,key=inp.count)
print(second)
```
**Input :**
```input
successes
```
**Output :**
```csharp
c or 'e' (both are correct as they appear the same number of times)

```
