# Chapter 7 Console Input/Output

<div class="chapter-social-card">
  <div class="chapter-info">
    <div class="chapter-number">CHAPTER 7</div>
    <h1 class="chapter-title">Console Input/Output</h1>
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

### 7.1 Console Input/Output

Console Input/Output means input from **keyboard** and output to **screen**.

### 7.2 Console Input

Console input can be received using the built-in `input( )` function.
General form of `input( )` function is `s = input('prompt')`
- prompt is a string that is displayed on the screen, soliciting a value. `input( )` returns a string. If 123 is entered as input, '123' is returned.
```python
# receive full name 
name = input('Enter full name') 
# separate first name, middle name and surname
fname, mname, lname = input('Enter full name: ').split( )
```
`split( )` function will split the entered fullname with space as a delimiter. The split values will then be assigned to `fname`, `mname`, `lname`.

If we are to receive multiple `int` values, we can receive them as strings and then convert them to `ints`.
```python title="Receiving multiple int values"
n1, n2, n3 = input('Enter three values: ').split( ) 
n1, n2, n3 = int(n1), int(n2), int(n3)
print(n1 + 10, n2 + 20, n3 + 30)
```

The same thing can be done using in a more compact manner using a feature called list comprehension. It applies `int( )` function to every element of the list returned by the `split( )` function. 
```python title="List Comprehension"
n1, n2, n3 = [int(n) for n in input('Enter three values: ').split( )] 
print(n1 + 10, n2 + 20, n3 + 30)
```
- The expression enclosed within [ ] is called list comprehension. It is discussed in detail in **Chapter 12.**

input( ) can be used to receive arbitrary number of values.
```python title="Receiving arbitrary number of values"
numbers = [int(x) for x in input('Enter values: ').split( )] 
for n in numbers :
    print(n + 10)
```
`input( )` can be used to receive different types of values at a time.
```python title="Receiving different types of values"
data = input('Enter name, age, salary: ').split( ) 
name = data[0]
age = int(data[1])
salary = float(data[2])
print(name, age, salary)
```
### 7.3 Console Output

- Built-in function `print( )` is used to send output to screen.

`print( )` function has this form:
```python
print(objects, sep = ' ', end = '\n', file = sys.stdout, flush = False)
```

- This means that by default objects will be printed on screen (sys.stdout), separated by space `(sep = ' ')` and last printed object will be followed by a newline (end = '\n'). `flush = False` indicates that output stream will not be flushed.

Python has a facility to call functions and pass keyword-based values as arguments. So while calling `print( )` we can pass specific values for `sep` and `end`. In this case, default values will not be used; instead the values that we pass will be used.
```python title="Keyword-based arguments"
print(a, b, c, sep = ',', end = '!') # prints ',' after each value, ! at end
print(x, y, sep = '...', end = '#') # prints '...' after each value, # at end
```

### 7.4 Formatted Printing

There are 4 ways to control the formatting of output:

- a. Using formatted string literals - easiest
- b. Using the format( ) method - older
- c. C printf( ) style - legacy
- d. Using slicing and concatenation operation - difficult

Today (a) is most dominantly used method followed by (b).
```python
r, l, b = 1.5678, 10.5, 12.66
print(f'radius = {r}')
print(f'length = {l} breadth = {b} radius = {r}')

name = 'Sushant Ajay Raje'
for n in name.split( ) :
    print(f'{n:10}') # print in 10 columns
```
Using format( ) method of string object:
```python title="Using format( ) method"
r, l, b = 1.5678, 10.5, 12.66
name, age, salary = 'Rakshita', 30, 53000.55

# print in order by position of variables using empty {}
print('radius = {} length = {} breadth ={}'.format(r, l, b))
print('name = {} age = {} salary = {}'.format(name, age, salary))

# print in any desired order
print('radius = {2} length = {1} breadth ={0}'.format(r, l, b))
print('age={1} salary={2} name={0}'.format(name, age, salary))

# print name in 15 columns, salary in 10 columns
print('name = {0:15} salary = {1:10}'.format(name, salary))

# print radius in 10 columns, with 2 digits after decimal point
print('radius = {0:10.2f}'.format(r))
```

- On execution, the above code snippet will produce the following output:
```python
radius = 1.5678 length = 10.5 breadth =12.66
name = Rakshita age = 30 salary = 53000.55
radius = 12.66 length = 10.5 breadth =1.5678
age=30 salary=53000.55 name=Rakshita
name = Rakshita salary = 53000.55
radius = 1.57
```

## **Problems**

### **Problem 7.1**

Write a program to receive radius of a circle, and length and breadth of a rectangle in one call to `input( )`. Calculate and print the circumference of circle and perimeter of rectangle.

<details>
<summary>Program</summary>

```python 
r, l, b = input('Enter radius, length and breadth: ').split( ) 
radius = int(r)
length = int(l)
breadth = int(b)
circumference = 2 * 3.14 * radius 
perimeter = 2 * ( length + breadth ) 
print(circumference)
print(perimeter)
```
</details>

<details>
<summary>Output</summary>

```python
Enter radius, length and breadth: 3 4 5
18.84
18
```
</details>

!!! tips "Tips"
    - `input( )` returns a string, so it is necessary to convert it into int or float suitably, before performing arithmetic operations.


### Problem 7.2

Write a program to receive 3 integers using one call to `input( )`. The three integers signify starting value, ending value and step value for a range. The program should use these values to print the number, its square and its cube, all properly right-aligned. Also output the same values left-aligned.

<details>
<summary>Program</summary>

```python 
start, end, step = input('Enter start, end, step values: ').split( )
# right aligned printing
for n in range(int(start), int(end), int(step)) :
print(f'{n:>5}{n**2:>7}{n**3:>8}')
print( ) 

# left aligned printing
for n in range(int(start), int(end), int(step)) :
print('{0:<5}{1:<7}{2:<8}'.format(n, n ** 2, n ** 3))
```
</details>

<details>
<summary>Output</summary>

```python
Enter start, end, step values: 1 10 2
1 1 1
3 9 27
5 25 125
7 49 343
9 81 729

1 1 1 
3 9 27 
5 25 125 
7 49 343 
9 81 729 
```
</details>

!!! tips "Tips"
    - `{n:>5}` will print n right-justified within 5 columns. Use `<` to left-justify.
    - `{0:<5}` will left-justify 0th parameter in the list within 5 columns. Use `>` to right-justify.


### Problem 7.3

Write a program to maintain names and cell numbers of 4 persons and then print them systematically in a tabular form.

<details>
<summary>Program</summary>

```python 
contacts = {

'David' : 9823077892, 'Shine' : 6784512345,
'Vivad' : 9823011245, 'Rosanna' : 9766556779 

}
for name, cellno in contacts.items( ) :
print(f'{name:15} : {cellno:10d}')
```
</details>

<details>
<summary>Output</summary>

```python
David : 9823077892
Shine : 6784512345
Vivad : 9823011245
Rosanna : 9766556779
```
</details>

### Problem 7.4

Suppose there are 5 variables in a program—max, `min`, `mean`, `sd` and `var`, having some suitable values. Write a program to print these variables properly aligned using multiple `fstrings`, but one call to `print( )`. 


<details>
<summary>Program</summary>

```python 
min, max = 25, 75
mean = 35
sd = 0.56
var = 0.9
print(
    f'\n{"Max Value:":<15}{max:>10}',
    f'\n{"Min Value:":<15}{min:>10}',
    f'\n{"Mean:":<15}{mean:>10}',
    f'\n{"Std Dev:":<15}{sd:>10}',
    f'\n{"Variance:":<15}{var:>10}' )
```
</details>

<details>
<summary>Output</summary>

```python
Max Value: 75 
Min Value: 25 
Mean: 35 
Std Deviation: 0.56 
Variance: 0.9
```
</details>

### Problem 7.5

Write a program that prints square root and cube root of numbers from 1 to 10, up to 3 decimal places. Ensure that the output is displayed in separate lines, with number center-justified and square and cube roots, right-justified.

<details>
<summary>Program</summary>

```python 
import math
width = 10
precision = 4
for n in range(1, 10) :
s = math.sqrt(n)
c = math.pow(n,1/3)
print(f'{n:^5}{s:{width}.{precision}}{c:{width}.{precision}}')
```
</details>

<details>
<summary>Output</summary>

```python
1 1.0 1.0
2 1.414 1.26
3 1.732 1.442
4 2.0 1.587
5 2.236 1.71
6 2.449 1.817
7 2.646 1.913
8 2.828 2.0
9 3.0 2.08
```
</details>


## **Exercises**

### **[A] Attempt the following questions:**

a. How will you make the following code more compact?
```python
print('Enter ages of 3 persons')
age1 = input( )
age2 = input( )
age3 = input( )
```

b. How will you print "Rendezvous" in a line and retain the cursor in the same line in which the output has been printed?

c. What will be the output of the following code snippet? 
```python
l, b = 1.5678, 10.5
print('length = {l} breadth = {b}')
```

d. In the following statement what do > 5, > 7 and > 8 signify?
```python
print(f'{n:>5}{n ** 2:>7}{n ** 3:>8}')
```

e. What will be the output of the following code segment?
```python
name = 'Shine'
cellno = 9823017892
print(f'{name:15} : {cellno:10}')
```

f. How will you print the output of the following code segment using fstring?
```python
x, y, z =10, 20, 40
print('{0:<5}{1:<7}{2:<8}'.format(x, y, z))
```

g. How will you receive arbitrary number of floats from keyboard?

h. What changes should be made in 
```python
print(f'{'\nx = ':4}{x:>10}{'\ny = ':4}{y:>10}')
to produce the output given below:
x = 14.99 
y = 114.39 
```

i. How will you receive a boolean value as input?

j. How will you receive a complex number as input?

k. How will you display price in 10 columns with 4 places beyond decimal points? Assume value of price to be 1.5567894.

l. Write a program to receive an arbitrary number of floats using one `input( )` statement. Calculate the average of floats received.

m. Write a program to receive the following using one `input( )` statement. 
```python 
Name of the person
Years of service
Diwali bonus received
Calculate and print the agreement deduction as per the following 
formula:
deduction = 2 * years of service + bonus * 5.5 / 100
```

n. Which import statement should be added to use the built-in functions `input( )` and `print( )`?

o. Is the following statement correct?
```python
print('Result = ' + 4 > 3)
```
p. Write a program to print the following values
```python
a = 12.34, b = 234.39, c = 444.34, d = 1.23, e = 34.67
```
as shown below:
```python
a = 12.34 
b = 234.39 
c = 444.34 
d = 1.23 
e = 34.67
```
### **[B] Match the following pairs:**
|Option A|Option B|
|---|---|
|a. Default value of sep in print( ) |1. `' '`|
|b. Default value of end in print( ) |2. `Using fstring`|
|c. Easiest way to print output |3. Right justify num in 5 columns|
|d. Return type of split( ) |4. Left justify num in 5 columns|
|e. print('{num:>5}') |5. list|
|f. print('{num:<5}') |6. `\n`|


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
