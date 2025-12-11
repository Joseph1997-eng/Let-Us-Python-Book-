# Chapter 8 Lists

<div class="chapter-social-card">
  <div class="chapter-info">
    <div class="chapter-number">CHAPTER 8</div>
    <h1 class="chapter-title">Lists</h1>
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

### 8.1 Lists

Container is an entity which contains multiple data items. It is also known as a collection or a compound data type. 

Python has following container data types: 

- Lists Tuples 
- Sets Dictionaries 

A list can grow or shrink during execution of the program. Hence it is also known as a dynamic array. Because of this nature of lists they are commonly used for handling variable length data. 

A list is defined by writing comma-separated elements within [ ]. 
```python title="Defining lists"
num = [10, 25, 30, 40, 100] 
names = ['Shine', 'Anna', 'Rosanna', 'Superior'] 
```

List can contain dissimilar types, though usually they are a collection of similar types. For example: 
```python title="List containing dissimilar types"
animal = ['Zebra', 155.55, 110] 
```

Items in a list can be repeated, i.e. a list may contain duplicate items. 
Like printing, `*` can be used to repeat an element multiple times. An empty list is also feasible. 
```python title="Repeating list elements"
ages = [25, 26, 25, 27, 26] # duplicates allowed 
num = [10] * 5 # stores [10, 10, 10, 10, 10] 
lst = [ ] # empty list, valid 
```

### 8.2 Accessing List Elements 

Entire list can be printed by just using the name of the list. 
```python title="Printing list"
l = ['Able', 'was', 'I', 'ere', 'I', 'saw', 'elbA'] 
print(l) 
```
Like strings, individual elements in a list can be accessed using indices. Hence they are also known as sequence types. The index value starts from 0. 
```python title="Accessing list elements"
print(animals[1], ages[3])  
```
Like strings, lists can be sliced. 
```python title="Slicing lists"
print(animals[1:3]) 
print(ages[3:]) 
```
### 8.3 Looping in Lists 
If we wish to process each item in the list, we should be able to iterate through the list. This can done using a while or for loop. 
```python title="Looping through a list"
animals = ['Zebra', 'Tiger', 'Lion', 'Jackal', 'Kangaroo'] 
# using while loop 
i = 0 
while i < len(animals) : 
print(animals[ i ]) 
i += 1 
# using more convenient for loop 
for a in animals : 
print(a) 
```
While iterating through a list using a for loop, if we wish to keep track of index of the element that a is referring to, we can do so using the built-in `enumerate( )` function. 
```python title="Iterating through a list using enumerate()"
animals = ['Zebra', 'Tiger', 'Lion', 'Jackal', 'Kangaroo'] 
for index, a in enumerate(animals) : 
print(index, a) 
```

### 8.4 Basic List Operations 

**Mutability** - Unlike strings, lists are mutable (changeable). So lists can be updated as shown below: 
```python title="Mutating lists"
animals = ['Zebra', 'Tiger', 'Lion', 'Jackal', 'Kangaroo'] 
ages = [25, 26, 25, 27, 26, 28, 25] 
animals[2] ='Rhinoceros' 
ages[5] = 31 
ages[2:5] = [24, 25, 32] # sets items 2 to 5 with values 24, 25, 32 
ages[2:5] = [ ] # delete items 2 to 4 
```

**Concatenation** - One list can be concatenated (appended) at the end of another as shown below: 
```python title="Concatenating lists"
lst = [12, 15, 13, 23, 22, 16, 17] 
lst = lst + [33, 44, 55] 
print(lst) # prints [12, 15, 13, 23, 22, 16, 17, 33, 44, 55] 
```
**Merging** - Two lists can be merged to create a new list. 
```python title="Merging lists"
s = [10, 20, 30] 
t = [100, 200, 300] 
z = s + t 
print(z) # prints [10, 20, 30, 100, 200, 300] 
```

**Conversion** - A string/tuple/set can be converted into a list using the `list( )` conversion function. 
```python title="Converting string to list"
lst = list('Africa') # converts the string to a list ['A', 'f', 'r', 'i', 'c', 'a'] 
```

**Aliasing** - On assigning one list to another, both refer to the same list. Changing one changes the other. This assignment is often known as shallow copy or aliasing. 
```python title="Aliasing a list"
lst1 = [10, 20, 30, 40, 50] 
lst2 = lst1 # doesn't copy list. lst2 refers to same list as lst1 
print(lst1) # prints [10, 20, 30, 40, 50] 
print(lst2) # prints [10, 20, 30, 40, 50] 
lst1[0] = 100 
print(lst1[0], lst2[0]) # prints 100 100 
```         

**Cloning** - This involves copying contents of one list into another. After copying both refer to different lists, though both contain same values. Changing one list, doesn't change another. This operation is often known as deep copy. 
```python title="Cloning a list"
lst1 = [10, 20, 30, 40, 50] 
lst2 = [ ] # empty list 
lst2 = lst2 + lst1 # lst1, lst2 refer to different lists 
print(lst1) # prints [10, 20, 30, 40, 50] 
print(lst2) # prints [10, 20, 30, 40, 50] 
lst1[0] = 100 
print(lst1[0], lst2[0]) # prints 100, 10
```
**Searching** - An element can be searched in a list using the in membership operator as shown below: 
```python title="Searching in a list"
lst = ['a', 'e', 'i', 'o', 'u'] 
res = 'a' in lst # return True since 'a' is present in list 
res = 'z' not in lst # return True since 'z' is absent in list 
```

**Identity** - Whether the two variables are referring to the same list can be checked using the is identity operator as shown below: 
```python title="Checking identity of lists"
lst1 = [10, 20, 30, 40, 50] 
lst2 = [10, 20, 30, 40, 50] 
lst3 = lst1 
print(lst1 is lst2) # prints False 
print(lst1 is lst3) # prints True 
print(lst1 is not lst2) # prints True 
```
- Note the difference for basic types like int or str: 
```python title="Checking identity of basic types"
num1 = 10 
num2 = 10 
s1 = 'Hi' 
s2 = 'Hi' 
print( num1 is num2) # prints True 
print( s1 is s2) # prints True 
```

**Comparison** - It is possible to compare contents of two lists. Comparison is done item by item till there is a mismatch. In following code it would be decided that a is less than b when 3 and 5 are compared. 
```python title="Comparing lists"
a = [1, 2, 3, 4] 
b = [1, 2, 5] 
print(a < b) # prints True 
```

**Emptiness** - We can check if a list is empty using not operator. 
```python title="Checking emptiness of a list"
lst = [ ] 
if not lst : 
print('Empty list') 
```

- Alternately, we can convert a list to a bool and check the result. 

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
