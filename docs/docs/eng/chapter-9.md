# Chapter 9 Tuples

<div class="chapter-social-card">
  <div class="chapter-info">
    <div class="chapter-number">CHAPTER 9</div>
    <h1 class="chapter-title">Tuples</h1>
  </div>
  <div class="chapter-logo">
    <img src="/Let-Us-Python-Book-/Logo.png" alt="Let Us Python Book Logo">
  </div>
  <div class="chapter-social-links">
    <a href="https://github.com/Joseph1997-eng" target="_blank" class="social-icon" title="GitHub">
      <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" fill="currentColor" viewBox="0 0 16 16">
        <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/>
      </svg>
    </a>
    <a href="https://www.linkedin.com/in/robinson-joseph-61734a17a/" target="_blank" class="social-icon" title="LinkedIn">
      <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" fill="currentColor" viewBox="0 0 16 16">
        <path d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854V1.146zm4.943 12.248V6.169H2.542v7.225h2.401zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248-.822 0-1.359.54-1.359 1.248 0 .694.521 1.248 1.327 1.248h.016zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016a5.54 5.54 0 0 1 .016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225h2.4z"/>
      </svg>
    </a>
    <a href="https://www.facebook.com/josephsaimonn" target="_blank" class="social-icon" title="Facebook">
      <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" fill="currentColor" viewBox="0 0 16 16">
        <path d="M16 8.049c0-4.446-3.582-8.05-8-8.05C3.58 0-.002 3.603-.002 8.05c0 4.017 2.926 7.347 6.75 7.951v-5.625h-2.03V8.05H6.75V6.275c0-2.017 1.195-3.131 3.022-3.131.876 0 1.791.157 1.791.157v1.98h-1.009c-.993 0-1.303.621-1.303 1.258v1.51h2.218l-.354 2.326H9.25V16c3.824-.604 6.75-3.934 6.75-7.951z"/>
      </svg>
    </a>
  </div>
</div>

## Keynote

### 9.1 Tuples

What are Tuples?

- Though a list can store dissimilar data, it is commonly used for storing similar data.
- Though a tuple can store similar data it is commonly used for storing dissimilar data. The tuple data is enclosed within ( ) as shown below

```python title="Defining tuples"
a = ( ) # empty tuple
b = (10,) # tuple with one item. , after 10 is necessary
c = ('Sunny', 25, 34555.50) # tuple with dissimilar items
d = (10, 20, 30, 40) # tuple with similar items
```

- While creating the tuple `b`, if we do not use the comma after 10, `b` is treated to be of type `int`.

While initializing a tuple, we may `drop ( )`.
```python title="Defining tuples"
c = 'Sunny', 25, 34555.50 # tuple with multiple items
print(type(c)) # c is of the type tuple
```

Items in a tuple can be repeated, i.e. tuple may contain duplicate items. However, unlike list, tuple elements cannot be repeated using a `*`.
```python title="Defining tuples"
tpl1 = (10,) * 5 # stores (10, 10, 10, 10, 10)
tpl2 = (10) * 5 # stores (50)
```

### 9.2 Accessing Tuple Elements

Entire tuple can be printed by just using the name of the tuple.

```python title="Defining tuples"
tpl = ('Sunny', 25, 34555.50) 
print(tpl)
```

Tuple is an ordered collection. So order of insertion of elements in a tuple is same as the order of access. So like a string and list, tuple items too can be accessed using indices, starting with 0.

```python title="Defining tuples"
msg = ('Handle', 'Exceptions', 'Like', 'a', 'boss')
print(msg[1], msg[3])
```

Like strings and lists, tuples too can be sliced to yield smaller tuples.
```python title="Defining tuples"
emp = ('Sunny', 23, 23000, 1760, 2040)
print(emp[1:3]) # prints (23, 23000)
print(emp[3:]) # prints (1760, 2040)
print(emp[:3]) # prints ('Sunny', 23, 23000)
```
### 9.3 Looping in Tuples

If we wish to process each item in a tuple, we should be able to iterate through it. This can be done using a while loop or for loop.
```python title="Defining tuples"
tpl = (10, 20, 30, 40, 50)
i = 0
while i < len(tpl) :
    print(tpl[i])
    i += 1
for n in tpl :
    print(n)
```

While iterating through a tuple using a for loop, if we wish to keep track of index of the element that is being currently processed, we can do so using the built-in enumerate( ) function.
```python title="Defining tuples"
tpl = (10, 20, 30, 40, 50)
for index, n in enumerate(tpl) :
    print(index, n)
```

### 9.4 Basic Tuple Operations

Mutability - Unlike a list, a tuple is immutable, i.e. it cannot be modified.
```python title="Defining tuples"
msg = ('Fall', 'In', 'Line') 
msg[0] ='FALL' # error
msg[1:3] = ('Above', 'Mark') # error
```
Since a tuple is immutable operations like append, remove and insert do not work with a tuple.
```python title="Defining tuples"
msg = ('Fall', 'In', 'Line') 
msg.append('Like') # error
msg.remove('Line') # error
msg.insert(1, 'Above') # error
```

Though a tuple itself is immutable, it can contain mutable objects like lists.
```python
# mutable lists, immutable string—all can belong to tuple
s = ([1, 2, 3, 4], [4, 5], 'Ocelot')
```
If a tuple contains a list, the list can be modified since list is a mutable object. 
```python
s = ([1, 2, 3, 4], [10, 20], 'Oynx')
s[1][1] = 45 # changes first item of first list, i.e. 20
print(s) # prints ([1, 2, 3, 4], [4, 45], 'Oynx')

# one more way to change first item of first list
p = s[1]
p[1] = 100
print(s) # prints ([1, 2, 3, 4], [4, 100], 'Oynx')
```

The other basic operations that are done on a tuple are very similar to the ones done on a list. These operations are discussed in **Chapter 8**. You may try the following operations on tuples as an exercise:

- Concatenation
- Merging
- Conversion
- Aliasing
- Cloning
- Searching
- Identity
- Comparison
- Emptiness

### 9.5 Using Built-in Functions on Tuples

Many built-in functions can be used with tuples.
```python 
t = (12, 15, 13, 23, 22, 16, 17) # create tuple
len(t) # return number of items in tuple t
max(t) # return maximum element in tuple t
min(t) # return minimum element in tuple t
sum(t) # return sum of all elements in tuple t
any(t) # return True if any element of tpl is True
all(t) # return True if all elements of tpl are True
sorted(t) # return sorted list (not sorted tuple)
reversed(t) # used for reversing t
```

### 9.6 Tuple Methods

Any tuple is an object of type tuple. Its methods can be accessed using the syntax tpl.method( ). Usage of two methods is shown below:
```python
tpl = (12, 15, 13, 23, 22) # create tuple
print(tpl.count(23)) # return no. of times 23 appears in lst
print(tpl.index(22)) # return index of item 22
print(tpl.index(50)) # reports valueError as 50 is absent in lst
```

### 9.7 Tuple Varieties

It is possible to create a tuple of tuples.
```python
a = (1, 3, 5, 7, 9)
b = (2, 4, 6, 8, 10)
c = (a, b)
print(c[0][0], c[1][2]) # 0th element of 0th tuple, 2nd ele of 1st tuple

records = (

('Priya', 24, 3455.50), ('Sunny', 25, 4555.50), 
('Sunday', 25, 4505.50), ('Sonia', 27, 4455.55) 

) 
print(records[0][0], records[0][1], records[0][2])
print(records[1][0], records[1][1], records[1][2])
for n, a, s in records :
print(n,a,s)    
```
A tuple may be embedded in another tuple.
```python
x = (1, 2, 3, 4)
y = (10, 20, x, 30) 
print(y) # outputs (10, 20, (1, 2, 3, 4), 30)
```
It is possible to unpack a tuple within a tuple using the `*`operator.
```python
x = (1, 2, 3, 4) 
y = (10, 20, *x, 30)
print(y) # outputs (10, 20, 1, 2, 3, 4, 30)
```
It is possible to create a list of tuples, or a tuple of lists.

```python
lst = [('Priya', 24, 3455.50), ('Sunny', 25, 4555.50)]
tpl = (['Priya', 24, 3455.50], ['Sunny', 25, 4555.50])
```
If we wish to sort a list of tuples or tuple of lists, it can be done as follows:
```python
import operator
# each embedded tuple/list contains name, age, salary
lst = [('Shailesh', 24, 3455.50), ('Priyanka', 25, 4555.50)]
tpl = (['Shailesh', 24, 3455.50], ['Priyanka', 25, 4555.50])
print(sorted(lst))
print(sorted(tpl))
print(sorted(lst, key = operator.itemgetter(2)))
print(sorted(tpl, key = operator.itemgetter(2)))
```
By default, `sorted( )` sorts by first item in list/tuple, i.e. name. 

If we wish to sort by salary, we need to use the `itemgetter( )` function of operator module.

The key parameter of `sorted( )` requires a key function (to be applied to objects to be sorted) rather than a single key value.

`operator.itemgetter(2)` will give us a function that fetches salary from a list/tuple.

In general, `operator.itemgetter(n)` constructs a function that takes a list/tuple as input, and fetches the n-th element out of it.

## Problems

### Problem 8.1

Pass a tuple to the divmod( ) function and obtain the quotient and the remainder.

<details> <summary> Program </summary>

```python
result = divmod(17,3)
print(result)
t = (17, 3)
result = divmod(*t)
print(result)
```
</details>

<details>
<summary>Output</summary>

```python
(5, 2)
(5, 2)
```
</details>
!!! Tips "Tips"
    - If we pass t to divmod( ) an error is reported. We have to unpack the tuple into two distinct values and then pass them to `divmod( )`. `divmod( )` returns a tuple consisting of quotient and remainder.

### Problem 8.2

Write a Python program to perform the following operations:

- Pack first 10 multiples of 10 into a tuple
- Unpack the tuple into 10 variables, each holding 1 value
- Unpack the tuple such that first value gets stored in variable x, last value in y and all values in between into disposable variables _
- Unpack the tuple such that first value gets stored in variable i, last value in j and all values in between into a single disposable variable _

<details> <summary> Program </summary>

```python
tpl = (10, 20, 30, 40, 50, 60, 70, 8, 90, 100)
a, b, c, d, e, f, g, h, i, j = tpl
print(tpl)
print(a, b, c, d, e, f, g, h, i, j)
x, _, _, _, _, _, _, _, _, y = tpl
print(x, y, _)
i, *_, j = tpl
print(i, j, _)
```
</details>

<details>
<summary>Output</summary>

```python
(10, 20, 30, 40, 50, 60, 70, 8, 90, 100)
10 20 30 40 50 60 70 8 90 100
10 100 90
10 100 [20, 30, 40, 50, 60, 70, 8, 90]
```
</details>

!!! Tips "Tips"
    - Disposable variable _ is usally used when you do not wish to use the variable further, and is being used only as a place-holder.


### Problem 8.3

A list contains names of boys and girls as its elements. Boys' names are stored as tuples. Write a Python program to find out number of boys and girls in the list.

<details> <summary> Program </summary>

```python
lst = ['Susanne', 'Nancy', 'Joshua', ('Susan',), ('Rose',), 'Ryan']
boys = 0
girls = 0
for ele in lst:
   if isinstance(ele, tuple):
      boys += 1
   else :
      girls += 1
print('Boys = ', boys, 'Girls = ', girls)
```
</details>

<details>
<summary>Output</summary>

```python
Boys = 2 Girls = 4
```
</details>

!!! Tips "Tips"
    - `isinstance( )` functions checks whether ele is an instance of tuple type.
    - Note that since the tuples contain a single element, it is followed by a comma.


### Problem 8.4

A list contains tuples containing roll number, names and age of student. Write a Python program to gather all the names from this list into another list.

<details>
<summary> Program </summary>

```python
lst = [('A101', 'Susanne', 23), ('A104', 'Nancy', 25), ('A111', 'Joshua', 24)]
nlst = [ ]
for ele in lst:
nlst = nlst + [ele[1]]

print(nlst)
```
</details>

<details>
<summary>Output</summary>

```python
['Susanne', 'Nancy', 'Joshua']
```
</details>

!!! Tips "Tips"
    - `nlst` is an empty to begin with. During each iteration name is extracted from the tuple using `ele[1]` and added to the current list of names in `nlst`.


### Problem 8.5

Given the following tuple `('F', 'l', 'a', 'b', 'b', 'e', 'r', 'g', 'a', 's', 't', 'e', 'd')`, write a Python program to carry out the following operations:

- Add an ! at the end of the tuple
- Convert a tuple to a string
- Extract ('b', 'b') from the tuple
- Find out number of occurrences of 'e' in the tuple
- Check whether 'r' exists in the tuple
- Convert the tuple to a list
- Delete characters 'b, 'b', 'e', 'r' from the tuple

<details>
<summary> Program </summary>

```python
tpl = ('F', 'l', 'a', 'b', 'b', 'e', 'r', 'g', 'a', 's', 't', 'e', 'd')
# addition of ! is not possible as tuple is an immutable
# so to add ! we need to create a new tuple and then make tpl refer to it
tpl = tpl + ('!',)
print(tpl)
# convert tuple to string
s = ''.join(tpl)
print(s)

# extract ('b', 'b') from the tuple
t = tpl[3:5]
print(t)

# count number of 'e' in the tuple
count = tpl.count('e')
print('count = ', count)

# check whether 'r' exists in the tuple
print('r' in tpl)

# Convert the tuple to a list
lst = list(tpl)
print(lst)

# tuples are immutable, so we cannot remove elements from it
# we need to split the tuple, eliminate the unwanted element and then 
merge the tuples
tpl = tpl[:3] + tpl[7:]
print(tpl)
```
</details>

<details>
<summary>Output</summary>

```python
('F', 'l', 'a', 'b', 'b', 'e', 'r', 'g', 'a', 's', 't', 'e', 'd', '!')
Flabbergasted!
('b', 'b')
count = 2
True
['F', 'l', 'a', 'b', 'b', 'e', 'r', 'g', 'a', 's', 't', 'e', 'd', '!']
('F', 'l', 'a', 'g', 'a', 's', 't', 'e', 'd', '!')
```
</details>


## **Exercises**

### **[A] Which of the following properties apply to string, list and tuple?**

- Iterable
- Sliceable
- Indexable
- Immutable
- Sequence
- Can be empty
- Sorted collection
- Ordered collection
- Unordered collection
- Elements can be accessed using their position in the collection

### **[B] Which of the following operations can be performed on string, list and tuple?**

- a = b + c
- a += b
- Appending a new element at the end
- Deletion of an element at the 0th position
- Modification of last element
- In place reversal

### **[C] Answer the following questions:**

a. Is this a valid tuple? `tpl = ('Square')`

b. What will be the output of the following code snippet? 

```python
num1 = num2 = (10, 20, 30, 40, 50)
print(id(num1), type(num2))
print(isinstance(num1, tuple))
print(num1 is num2)
print(num1 is not num2)
print(20 in num1)
print(30 not in num2)
```

c. Suppose a date is represented as a tuple (d, m, y). Write a program to create two date tuples and find the number of days between the two dates.

d. Create a list of tuples. Each tuple should contain an item and its price in float. Write a program to sort the tuples in descending order by price. Hint: Use `operator.itemgetter( )`.

e. Store the data about shares held by a user as tuples containing the following information about shares:
```text
Share name
Date of purchase
Cost price
Number of shares
Selling price
```
Write a program to determine:

- Total cost of the portfolio.
- Total amount gained or lost.
- Percentage profit made or loss incurred.

f. Write a program to remove empty tuple from a list of tuples.

g. Write a program to create following 3 lists:

- a list of names
- a list of roll numbers 
- a list of marks

Generate and print a list of tuples containing name, roll number and marks from the 3 lists. From this list generate 3 tuples—one containing all names, another containing all roll numbers and third containing all marks.

### **[D] Match the following pairs:**

|Options A| Options B|
|---|---|
|`a. tpl1 = ('A',)` |1. tuple of length 6|
|`b. tpl1 = ('A')` |2. tuple of lists|
|`c. t = tpl[::-1]` |3. Tuple|
|`d. ('A', 'B', 'C', 'D')` |4. list of tuples|
|`e. [(1, 2), (2, 3), (4, 5)]` |5. String|
|`f. tpl = tuple(range(2, 5))` |6. Sorts tuple|
|`g. ([1, 2], [3, 4], [5, 6])` |7. (2, 3, 4)|
|`h. t = tuple('Ajooba')` |8. tuple of strings|
|`i. [*a, *b, *c]` |9. Unpacking of tuples in a list|
|`j. (*a, *b, *c)` |10. Unpacking of lists in a tuple|


---



<div class="comments-section">
  <h2 class="comments-title">💬 Comments & Discussion</h2>
  <script src="https://giscus.app/client.js"
        data-repo="Joseph1997-eng/Let-Us-Python-Book-"
        data-repo-id="R_kgDOQfXjHg"
        data-category="Announcements"
        data-category-id="DIC_kwDOQfXjHs4CzbEE"
        data-mapping="pathname"
        data-strict="0"
        data-reactions-enabled="1"
        data-emit-metadata="1"
        data-input-position="top"
        data-theme="preferred_color_scheme"
        data-lang="en"
        data-loading="lazy"
        crossorigin="anonymous"
        async>
  </script>
</div>
