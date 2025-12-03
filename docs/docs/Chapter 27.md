CHAPTER 27

# Numpy Library

## Table of Contents
- [Keynote](#keynote)
- [27.1 Creation of Array](#271-creation-of-array)
- [27.2 Creation of Filler Arrays](#272-creation-of-filler-arrays)
- [27.3 Array Attributes](#273-array-attributes)
- [27.4 Array Operations](#274-array-operations)
  - [27.4.1 Arithmetic Operations](#2741-arithmetic-operations)
  - [27.4.2 Statistical Operations](#2742-statistical-operations)
  - [27.4.3 Linear Algebra Operations](#2743-linear-algebra-operations)
  - [27.4.4 Bitwise Operations](#2744-bitwise-operations)
  - [27.4.5 Copying and Sorting](#2745-copying-and-sorting)
  - [27.4.6 Comparison](#2746-comparison)
  - [27.4.7 Indexing and Slicing](#2747-indexing-and-slicing)
- [27.5 Array Manipulation](#275-array-manipulation)
- [Problems](#problems)
- [Exercises](#exercises)

---

# Keynote
**[English]** 
- Numpy stands for Numerical Python. It is a popular library used for solving problems in science and engineering. It provides a high-performance multidimensional array object, and methods for fast operations on arrays, these operations include mathematical, logical, shape manipulation, sorting, selecting, I/O, statistical operations, etc.
---
**[Myanmar]** 
- NumPy ဆိုတာကတော့ Numerical Python ရဲ့ အတိုကောက်ဖြစ်ပြီး သိပ္ပံနဲ့ အင်ဂျင်နီယာပိုင်းဆိုင်ရာ ပြဿနာတွေကို ဖြေရှင်းတဲ့နေရာမှာ လူသုံးများတဲ့ Library တစ်ခုဖြစ်ပါတယ်။ သူက စွမ်းဆောင်ရည်မြင့်မားတဲ့ Multidimensional array object (ရှုထောင့်စုံ ဇယားကွက်) တွေနဲ့ အဲဒီ array တွေအပေါ်မှာ မြန်ဆန်သွက်လက်စွာ တွက်ချက်နိုင်မယ့် Method တွေကို ပံ့ပိုးပေးထားပါတယ်။ ဒီလိုလုပ်ဆောင်နိုင်တဲ့ လုပ်ငန်းစဉ်တွေထဲမှာ သင်္ချာဆိုင်ရာ၊ ယုတ္တိဗေဒ (Logic) ပိုင်း၊ ပုံသဏ္ဍာန် ပြုပြင်ပြောင်းလဲတာ၊ အစီအစဉ်ချတာ၊ ရွေးထုတ်တာ၊ Input/Output ကိစ္စတွေနဲ့ စာရင်းအင်း (Statistical) ပိုင်းဆိုင်ရာ တွက်ချက်မှုတွေ စသည်ဖြင့် ပါဝင်ပါတယ်။

## 27.1 Creation of Array 
**[English]**
- To use **Numpy Library**, it must be downloaded and installed as shown below: 
```bash 
pip install numpy
```
- Though Numpy Array looks like Python list, it is optimized to run faster than lists. 
- Unlike lists, all elements of a Numpy array are of the same type.
- To create a Numpy array we have to use the **np.array()** function and pass a list of numbers to it as shown below: 
```python 
import numpy as np 
intarr = np.array([1,2,3,4]) #creates array of ints
floattarr = np.array([1.1,2.2,3.3,4.4]) #creats array of floats
```
- If we mix ints and floats, Numpy defaults to array of flatts.
- While creating an array if we do not specify the type of elements in it, then from the values Numpy guesses the type. If we wish we can also specify the type. 
```python 
intarr = np.array([1,2,3,4],int)
floatarr = np.array([1.1,2.2,3.3,4.4], float)
```
- 2D array (matrix) is a collection of several 1D arrays and 3D array is a collection of several 2D arrrays. They can be created as shown below: 
```python 
a1 = np.array([[1,2,3],[4,5,6]]) # 2 rows x 3 col
a2 = np.array([[[1,2],[4,5]],[[6,7],[8,9]]]) # 2,2 x 2 arrays
```
- Array of complex numbers can also be created: 
```python 
c = np.array([[1,2],[3,4]],complex)
```

---
**[Myanmar]**
- NumPy Library ကို အသုံးပြုချင်တယ်ဆိုရင်တော့ အောက်မှာပြထားတဲ့အတိုင်း အရင်ဆုံး download ဆွဲပြီး install လုပ်ထားဖို့ လိုပါမယ်။
```Bash
pip install numpy
```
- NumPy Array တွေက ပုံစံကြည့်လိုက်ရင် Python List တွေနဲ့ တူသလိုလိုရှိပေမယ့်၊ တကယ်တမ်းကျတော့ List တွေထက် ပိုပြီး မြန်မြန်ဆန်ဆန် အလုပ်လုပ်နိုင်အောင် ဖန်တီးထားတာဖြစ်ပါတယ်။
- List တွေနဲ့ မတူတဲ့အချက်ကတော့ NumPy array တစ်ခုထဲမှာပါတဲ့ element တွေအားလုံးဟာ data type အမျိုးအစား တူညီနေဖို့ လိုပါတယ်။
- NumPy array တစ်ခု တည်ဆောက်ချင်ရင် np.array() function ကို သုံးရမှာဖြစ်ပြီး၊ အောက်ပါနမူနာအတိုင်း ကိန်းဂဏန်း list တစ်ခုကို ထည့်ပေးရပါမယ်။
```Python
import numpy as np 
intarr = np.array([1,2,3,4]) # ကိန်းပြည့် (ints) array တစ်ခု တည်ဆောက်ခြင်း
floattarr = np.array([1.1,2.2,3.3,4.4]) # ဒသမကိန်း (floats) array တစ်ခု တည်ဆောက်ခြင်း
```
- တကယ်လို့ ကိန်းပြည့် (ints) တွေနဲ့ ဒသမကိန်း (floats) တွေကို ရောရေးလိုက်မယ်ဆိုရင် NumPy က အားလုံးကို floats အဖြစ် အလိုအလျောက် ပြောင်းလဲသတ်မှတ်လိုက်မှာ ဖြစ်ပါတယ်။
- Array တည်ဆောက်တဲ့အချိန်မှာ element တွေရဲ့ type ကို သီးခြား မသတ်မှတ်ပေးထားဘူးဆိုရင် NumPy က ပေးထားတဲ့ တန်ဖိုးတွေကိုကြည့်ပြီး type ကို ခန့်မှန်းပေးပါတယ်။ တကယ်လို့ ကိုယ်တိုင် type သတ်မှတ်ချင်တယ်ဆိုရင်လည်း အခုလို သတ်မှတ်ပေးလို့ ရပါတယ်။
```Python
intarr = np.array([1,2,3,4], int)
floatarr = np.array([1.1,2.2,3.3,4.4], float)
```
- 2D array (matrix) ဆိုတာက 1D array တွေကို စုစည်းထားတာဖြစ်ပြီး၊ 3D array ဆိုတာကတော့ 2D array တွေကို ထပ်ပြီး စုစည်းထားတာ ဖြစ်ပါတယ်။ သူတို့ကို အောက်ပါအတိုင်း တည်ဆောက်နိုင်ပါတယ်။
```Python
a1 = np.array([[1,2,3],[4,5,6]]) # 2 rows x 3 columns ရှိတဲ့ array
a2 = np.array([[[1,2],[4,5]],[[6,7],[8,9]]]) # 2x2 အရွယ်အစားရှိတဲ့ array ၂ ခုပါဝင်တဲ့ 3D array
```
- Complex number (ကိန်းရော) တွေပါဝင်တဲ့ array တွေကိုလည်း တည်ဆောက်နိုင်ပါသေးတယ်။
```Python
c = np.array([[1,2],[3,4]], complex)
```
---

## 27.2 Creation of Filler Arrays 
**[English]**
- We can create Numpy Arrays which contain initial placeholder values, which can be replaced later. 
- For example, we can create arrays which are filled with all *0s*, all *1s* or a fixed value. We can even create empty arrays which are filled with garbage values. 

```python 
import numpy as np
a1 = np.empty((3,4))  # creates 2D array with garbage values 
a2 = np.zeros((3,4))  # creates 2D array of zeros. 
a3 = np.ones((3,4))   # creates 2D array of ones
a4 = np.full((2,2),7) # creates 2D array with all values set to 7
```
Note that tuples need to be passed to these functions. The tuples (3,4) and (2,2) indicates the shape of the array that we wish to create. 
- We can create arrays with random values or with evenly space values. 
```python 
import numpy as np
a1 = np.random.random((4))  # creates array with 4 random val
a2 = np.range(5)            # creates [0,1,2,3,4]
a3 = np.linspace(0,2,5)     # creates [0.0 0.5 1.0 1.5 2.0]
```
- The first two parameters of *arrange()* and *linspace()* indicate the starting an ending values. The third parameter of *arange()* indicates the setp value, whereas that of *linspace()* indicates number of values that wew wish to create. 
- Numpy allows us to create an identity matrix, a matrix in which all elements in the principal diagonal are ones, and all other elements are zeros. 
```python 
import numpy as np
a1 = np.eye(3)
a2 = np.identity(3)
```
- Since identity matrix is a square matrix we are required to apps only 1 dimension to *eye()* and *identity()*. 


**[Myanmar]**
- နောက်မှ တန်ဖိုးအစစ်တွေ အစားထိုးထည့်မယ့် နေရာဦးထားတဲ့ (initial placeholder) တန်ဖိုးတွေပါတဲ့ NumPy Array တွေကို ကြိုတင်တည်ဆောက်ထားလို့ ရပါတယ်။

- ဥပမာ - 0 တွေချည်းပဲပါတာ၊ 1 တွေချည်းပဲပါတာ၊ ဒါမှမဟုတ် ကိုယ်လိုချင်တဲ့ ဂဏန်းသေချာသတ်မှတ်ပြီး ဖြည့်ထားတဲ့ array မျိုးတွေ ဖန်တီးနိုင်တယ်။ ဘာတန်ဖိုးမှန်းမသိတဲ့ (garbage values) တွေပါနေတဲ့ empty array မျိုးကိုလည်း ဖန်တီးလို့ရပါတယ်။
```Python
import numpy as np
a1 = np.empty((3,4))  # garbage values တွေပါတဲ့ 2D array တစ်ခု
a2 = np.zeros((3,4))  # သုည (0) တွေချည်းပဲပါတဲ့ 2D array
a3 = np.ones((3,4))   # တစ် (1) တွေချည်းပဲပါတဲ့ 2D array
a4 = np.full((2,2),7) # တန်ဖိုးအားလုံး 7 ဖြစ်နေတဲ့ 2D array
```
သတိပြုရန် - ဒီ function တွေထဲကို တန်ဖိုးထည့်တဲ့အခါ Tuple ပုံစံနဲ့ ထည့်ပေးရပါမယ်။ (3,4) တို့ (2,2) တို့ဆိုတာ ကိုယ်တည်ဆောက်ချင်တဲ့ array ရဲ့ ပုံသဏ္ဍာန် (Shape) ကို ညွှန်းဆိုတာ ဖြစ်ပါတယ်။

- Random တန်ဖိုးတွေနဲ့ဖြစ်ဖြစ်၊ အကွာအဝေး ညီတူညီမျှခြားထားတဲ့ တန်ဖိုးတွေနဲ့ဖြစ်ဖြစ် array တွေကို တည်ဆောက်နိုင်ပါတယ်။
```Python
import numpy as np
a1 = np.random.random((4))   # random တန်ဖိုး ၄ ခုပါတဲ့ array
a2 = np.arange(5)            # [0,1,2,3,4] ကို ဖန်တီးပေးတယ် (မူရင်းစာ text တွင် np.range ဟုပါသော်လည်း np.arange သာ အမှန်ဖြစ်သည်)
a3 = np.linspace(0,2,5)      # [0.0 0.5 1.0 1.5 2.0] ကို ဖန်တီးပေးတယ်
```
- *arange()* နဲ့ *linspace()* ရဲ့ ပထမ ကိန်းဂဏန်းနှစ်လုံး (parameters) က အစတန်ဖိုးနဲ့ အဆုံးတန်ဖိုးကို ညွှန်းတာပါ။ တတိယ parameter မှာကျတော့ *arange()* အတွက်ဆိုရင် ဘယ်လောက်စီ ခြားမလဲဆိုတဲ့ step value ဖြစ်ပြီး၊ *linspace()* အတွက်ဆိုရင်တော့ တန်ဖိုးစုစုပေါင်း ဘယ်နှလုံး လိုချင်တာလဲ ဆိုတာကို ညွှန်းတာဖြစ်ပါတယ်။

- NumPy ကနေ Identity Matrix ကိုလည်း ဖန်တီးခွင့်ပေးထားပါတယ်။ Identity Matrix ဆိုတာက ထောင့်ဖြတ်မျဉ်း (principal diagonal) ပေါ်မှာ 1 တွေရှိပြီး ကျန်တဲ့နေရာတွေမှာ 0 ဖြစ်နေတဲ့ Matrix မျိုးပါ။
```Python
import numpy as np
a1 = np.eye(3)
a2 = np.identity(3)
```
- Identity matrix ဆိုတာ အနားညီစတုရန်း (Square) matrix ဖြစ်တဲ့အတွက် eye() နဲ့ identity() ကို သုံးတဲ့အခါ dimension တစ်ခုပဲ (ဂဏန်းတစ်လုံးပဲ) ထည့်ပေးဖို့ လိုပါတယ်။

## 27.3 Array Attributes
**[English]**
- A Numpy array has several attributes that indicate the element type, element size, shape of array, size of array, etc. 
- We can obtain the type of elements present in a Numpy array their size, their location in memory, etc. 
```python 
import numpy as np
a1 = np.array([1,2,3,4])
a2 = np.array([1.1,2.2,3.3,4.4])
print(a1.dtype)                 # prints int32
print(a2.dtype)                 # prints float64
print(a1.itemsize)              # prints 4
print(a2.itemsize)              # prints 8
print(a1.nbytes)                # prints 16
print(a2.nbytes)                # prints 16
print(a1.data)                  # prints <memory at 0x024BEE08>
print(a1.strides)               # prints (4,)
print(a2.data)                  # prints <memory at 0x0291EE08>
print(a2.strides)               # prints (8,)
```
- Here *dtype* specifies the type of elements contained in the array. Number of bytes occupied by individual array element and by entrie array are available through attributes *itemsize* and *nbytes*, respectively. 
- *data* gives the address in memory where the array begins (often called base address) and *strides* indicates the number of bytes that should be added to base address to reach the next array element. 
- Attributes *ndim*, *shape* and *size* yield the number of dimensions in the array the shape of the array and the number of elements in it. 
```python 
import numpy as np
a1 = np.array ([1,2,3,4])
a2 = np.array(([1,2,3,4],[5,6,7,8]))
print(a1.ndim)                       # prints 1
print(a2.ndim)                       # prints 2
print(a1.shape)                      # prints tuple (4,)
print(a2.shape)                      # prints tuple (2,4)
print(a1.size)                       # prints 4
print(a2.size)                       # prints 8
```
---
**[Myanmar]**
- NumPy array တွေမှာ သူ့ရဲ့ element အမျိုးအစား (type)၊ အရွယ်အစား (size)၊ ပုံသဏ္ဍာန် (shape) စတာတွေကို ဖော်ပြပေးနိုင်တဲ့ attribute တွေ အများကြီး ပါဝင်ပါတယ်။

- Array ထဲမှာ ဘာ data type တွေပါလဲ၊ size ဘယ်လောက်ရှိလဲ၊ memory ရဲ့ ဘယ်နေရာမှာ သိမ်းထားလဲ ဆိုတာတွေကို အောက်ပါအတိုင်း လှမ်းကြည့်လို့ရပါတယ်။
```Python
import numpy as np
a1 = np.array([1,2,3,4])
a2 = np.array([1.1,2.2,3.3,4.4])
print(a1.dtype)                 # int32 လို့ ထွက်လာမယ် (Integer type မို့လို့ပါ)
print(a2.dtype)                 # float64 လို့ ထွက်လာမယ် (Float type မို့လို့ပါ)
print(a1.itemsize)              # 4 လို့ ပြမယ် (bytes)
print(a2.itemsize)              # 8 လို့ ပြမယ် (bytes)
print(a1.nbytes)                # 16 (စုစုပေါင်း bytes)
print(a2.nbytes)                # 32 (မူရင်းစာ text တွင် 16 ဟုပါသော်လည်း float64 သည် 8 bytes x 4 elements ဖြစ်၍ 32 bytes ဖြစ်သင့်သည်)
print(a1.data)                  # Memory address ကို ပြပါလိမ့်မယ် (ဥပမာ <memory at ...>)
print(a1.strides)               # (4,) လို့ ပြမယ်
print(a2.data)                  # Memory address ကို ပြပါလိမ့်မယ်
print(a2.strides)               # (8,) လို့ ပြမယ်
```
- ဒီမှာဆိုရင် *dtype* က array ထဲမှာပါတဲ့ element အမျိုးအစားကို ပြပေးတာပါ။ Element တစ်လုံးချင်းစီက နေရာဘယ်လောက်ယူလဲဆိုတာကို *itemsize* နဲ့ ကြည့်နိုင်ပြီး၊ Array တစ်ခုလုံးအနေနဲ့ နေရာဘယ်လောက်ယူလဲ ဆိုတာကိုတော့ nbytes နဲ့ ကြည့်နိုင်ပါတယ်။
- *data* ဆိုတာက memory ပေါ်မှာ array စတင်သိမ်းဆည်းထားတဲ့ လိပ်စာ (Base Address) ကို ပြပေးတာဖြစ်ပြီး၊ *strides* ကတော့ နောက်ထပ် element တစ်ခုဆီ ရောက်ဖို့အတွက် base address ကနေ byte ဘယ်လောက် ထပ်ပေါင်းထည့်ရမလဲ (ဘယ်လောက် ခုန်ကျော်သွားရမလဲ) ဆိုတာကို ညွှန်းပါတယ်။
- *ndim*, *shape* နဲ့ *size attributes* တွေကတော့ array ရဲ့ dimension အရေအတွက်၊ array ရဲ့ ပုံသဏ္ဍာန်နဲ့ element စုစုပေါင်း အရေအတွက်တွေကို အသီးသီး ဖော်ပြပေးပါတယ်။
```Python
import numpy as np
a1 = np.array ([1,2,3,4])
a2 = np.array(([1,2,3,4],[5,6,7,8]))

print(a1.ndim)                       # 1 (1D array ဖြစ်လို့)
print(a2.ndim)                       # 2 (2D array ဖြစ်လို့)
print(a1.shape)                      # (4,) (Tuple ပုံစံနဲ့ ပြပါတယ်)
print(a2.shape)                      # (2,4) (2 rows နဲ့ 4 columns ရှိလို့ပါ)
print(a1.size)                       # 4 (element ၄ လုံးရှိလို့)
print(a2.size)                       # 8 (element ၈ လုံးရှိလို့)
```

## 27.4 Array Operations 
**[English]**
- Many operations can be performed on Numpy arrays. These operations are compact and fast. The speed is achieved through the already precompiled routines present in the library. 
- The different array operations include the following: 
    - (a) Arithmetic Operations
    - (b) Statistical Operations
    - (c) Linear Algebra Operations
    - (d) Bitwise Operations 
    - (e) Copying, Sorting 
    - (f) Comparsion Operations

**Array Operations (Array ဆိုင်ရာ လုပ်ဆောင်ချက်များ)**

**[Myanmar]**
- NumPy Array တွေပေါ်မှာ လုပ်ဆောင်ချက် (Operations) တွေ အများကြီး လုပ်လို့ရပါတယ်။ ဒီ operations တွေက ရေးရတာ ကျစ်လျစ်သလို၊ အလုပ်လုပ်တာလည်း အရမ်းမြန်ပါတယ်။ ဘာလို့ ဒီလောက်မြန်လဲဆိုတော့ ဒီ Library ထဲမှာ ကြိုတင် compile လုပ်ပြီးသား ကုဒ်တွေ (precompiled routines) ပါနေလို့ပဲ ဖြစ်ပါတယ်။

- Array operations အမျိုးမျိုးရှိတဲ့အထဲမှာ အောက်ပါခေါင်းစဉ်တွေ ပါဝင်ပါတယ် -

    - (a) Arithmetic Operations: သင်္ချာဆိုင်ရာ ပေါင်းနှုတ်မြှောက်စား လုပ်ဆောင်ချက်များ
    - (b) Statistical Operations: စာရင်းအင်းပိုင်းဆိုင်ရာ တွက်ချက်မှုများ
    - (c) Linear Algebra Operations: Linear Algebra (ရိုးဖြောင့် အက္ခရာသင်္ချာ) ဆိုင်ရာ တွက်ချက်မှုများ
    - (d) Bitwise Operations: Bit အလိုက် ကိုင်တွယ်တဲ့ လုပ်ဆောင်ချက်များ
    - (e) Copying, Sorting: ကူးယူခြင်း နဲ့ အစီအစဉ်ချခြင်းများ
    - (f) Comparison Operations: နှိုင်းယှဉ်ခြင်းဆိုင်ရာ လုပ်ဆောင်ချက်များ

### 27.4.1 Arithmetic Operations
**[English]**
- You can perform many operations like +,-,*,/,% on two arrays.When we use these operators, ther operations are performed on corresponding elements of the two arrays. Instead of using these operators, you may also use methods like **add()**, **subtract()**, **multiply()**, **divide()**, and **remainder()**. These operations are often known as vector operations. 
```python
import numpy as np
a1 = np.array([[10,2,3,4],[5,6,7,8]])
a2 = np.array([[1,1,1,1],[2,2,2,2]])
a3 = a1 + a2                            # same as a3 = np.add(a1,a2)
a4 = a1 - a2
a5 = a1 * a2
a6 = a1 / a2
a7 = a1 % a2 
a8 = a1 ** 2                            # raises every element to a power of 2
```
- We can perform scalar arithmetic operations on array elements. 
```python
import numpy as np
a1 = np.array([[10,2,3,4],[5,6,7,8]])
a2 = a1 + 2             # adds 2 to every element
a3 = a1 **2             # raises every element to a power of 2
```
- In place operators +=,-=, /= modify an existing array, instead of creating a new one. 
```python
a1 += a2 # is same as a1 = a1 + a2
a3 += 5  # is same as a3 = a3 + 5
```
- Other operations that can be done on array elements include **exp()**, **sqrt()**, **cos()**, **sin()**, **log()**. 

---
**Arithmetic Operations (သင်္ချာဆိုင်ရာ တွက်ချက်မှုများ)**

**[Myanmar]**
- Array နှစ်ခုကြားမှာ +, -, *, /, % စတဲ့ သင်္ချာ operator တွေကို အသုံးပြုပြီး တွက်ချက်မှုတွေ အများကြီး လုပ်လို့ရပါတယ်။

- ဒီ operator တွေကို သုံးလိုက်တဲ့အခါ Array နှစ်ခုရဲ့ သက်ဆိုင်ရာ နေရာတူ element အချင်းချင်း (corresponding elements) ကို တိုက်ရိုက် တွက်ချက်သွားမှာ ဖြစ်ပါတယ်။

- သင်္ကေတ (operator) တွေ မသုံးချင်ဘူးဆိုရင် **add()**, **subtract()**, **multiply()**, **divide()**, နဲ့ **remainder()** ဆိုတဲ့ function (method) တွေကို ပြောင်းသုံးလို့လည်း ရပါတယ်။ ဒီလို တွက်ချက်တာမျိုးကို Vector operations လို့လည်း ခေါ်ကြပါတယ်။
```Python
import numpy as np
a1 = np.array([[10,2,3,4],[5,6,7,8]])
a2 = np.array([[1,1,1,1],[2,2,2,2]])
a3 = a1 + a2                            # a3 = np.add(a1,a2) နဲ့ အတူတူပါပဲ
a4 = a1 - a2
a5 = a1 * a2
a6 = a1 / a2
a7 = a1 % a2 
a8 = a1 ** 2                            # Element တိုင်းကို နှစ်ထပ်ကိန်း တင်လိုက်တာပါ
```
- Array ထဲက element တွေကို ကိန်းဂဏန်းတစ်ခုတည်း (Scalar) နဲ့ ပေါင်းနှုတ်မြှောက်စား လုပ်တာမျိုးလည်း လုပ်လို့ရပါသေးတယ်။ (ဥပမာ - Array တစ်ခုလုံးကို 2 နဲ့ လိုက်ပေါင်းတာမျိုးပေါ့)
```Python
import numpy as np
a1 = np.array([[10,2,3,4],[5,6,7,8]])
a2 = a1 + 2             # Element တိုင်းကို 2 ပေါင်းထည့်လိုက်တာ
a3 = a1 ** 2            # Element တိုင်းကို 2 ထပ်ကိန်း တင်လိုက်တာ
```
- +=, -=, /= စတဲ့ In-place operator တွေကို သုံးမယ်ဆိုရင်တော့ Array အသစ်တစ်ခု ထပ်မဆောက်တော့ဘဲ ရှိပြီးသား လက်ရှိ Array ကိုပဲ တိုက်ရိုက် ပြင်ဆင် (Modify) သွားမှာ ဖြစ်ပါတယ်။
```Python
a1 += a2 # a1 = a1 + a2 နဲ့ အတူတူပါပဲ (a1 ရဲ့ တန်ဖိုးကို တိုက်ရိုက်ပြောင်းသွားပါတယ်)
a3 += 5  # a3 = a3 + 5 နဲ့ အတူတူပါပဲ
```
- Array element တွေအပေါ်မှာ တခြားလုပ်ဆောင်နိုင်တဲ့ operation တွေကတော့ **exp()** (ထပ်ကိန်းတင်ခြင်း)၊ **sqrt()** (နှစ်ထပ်ကိန်းရင်းရှာခြင်း)၊ **cos()**, **sin()** (တြီဂိုနိုမေတြီ တွက်ချက်ခြင်း) နဲ့ **log()** (Logarithm တွက်ချက်ခြင်း) စတာတွေပဲ ဖြစ်ပါတယ်။

### 27.4.2 Statistical Operations

**[English]**
- Numpy can perform following operations either on all elements of the array or on the elements of the specified axis. Note that axis means dimension, so a 1D array has 1 axis, a 2D array has 2 axes and so on. 
```python
import numpy as np
a = np.array([[1,2,3,],[4,5,6]])
print(a.sum())
print(a.min())                      # finds minimum in array
print(a.max(axis = 0))              # finds maximum in each column
print(a.max(axis = 1))              # finds maximum in each row
print(a.sum(axis = 1))              # sum along axis 1
print(a.cumsum(axis = 1))           # cumulative sum
print(np.mean(a))
print(np.median(a))
print(np.corrcoef(a))
print(np.std(a))
```
- It is imprtant to understand the use of axis in calls to **max()**. Our array is a 2D array of dimensions 2 x 3. When we use axis = 0, don't think about this as 'max along columns' or 'max along rows'. Instead, think that when we use axis = 0, Numpy finds maximum by condensing (or collapsing) size 2. So, result is an array containing 3 elements [4,5,6]. Similarly, when we use axis = 1, Numpy condenses size 3, resulting in an array containing elements [3,6]. 

---
**Statistical Operations (စာရင်းအင်းဆိုင်ရာ တွက်ချက်မှုများ)**

**[Myanmar]**
- NumPy က Array တစ်ခုလုံးအပေါ်မှာဖြစ်ဖြစ်၊ ကိုယ်လိုချင်တဲ့ Axis (Dimension) တစ်ခုပေါ်မှာ မူတည်ပြီးတော့ဖြစ်ဖြစ် စာရင်းအင်းဆိုင်ရာ တွက်ချက်မှုတွေ (ဥပမာ - ပေါင်းခြင်း၊ အကြီးဆုံးရှာခြင်း) ကို လုပ်ပေးနိုင်ပါတယ်။

- Axis ဆိုတာ Dimension (အတိုင်းအတာ) ကို ပြောတာပါ။ ဒါကြောင့် 1D array မှာ 1 axis ရှိပြီး၊ 2D array မှာ 2 axes ရှိတယ်လို့ မှတ်သားနိုင်ပါတယ်။
```Python
import numpy as np
a = np.array([[1,2,3,],[4,5,6]])
print(a.sum())
print(a.min())                      # Array တစ်ခုလုံးရဲ့ အငယ်ဆုံးတန်ဖိုးကို ရှာမယ်
print(a.max(axis = 0))              # Column တစ်ခုစီအလိုက် အကြီးဆုံးကို ရှာမယ်
print(a.max(axis = 1))              # Row တစ်ခုစီအလိုက် အကြီးဆုံးကို ရှာမယ်
print(a.sum(axis = 1))              # Axis 1 (Row) အတိုင်း ပေါင်းမယ်
print(a.cumsum(axis = 1))           # ဆင့်ပေါင်း (Cumulative sum) ရလဒ်ကို ထုတ်ပေးမယ်
print(np.mean(a))                   # ပျမ်းမျှတန်ဖိုး (Mean)
print(np.median(a))                 # အလယ်ကိန်း (Median)
print(np.corrcoef(a))               # Correlation Coefficient (ဆက်နွယ်မှု ကိန်းညွှန်း)
print(np.std(a))                    # Standard Deviation (စံသွေဖည်ကိန်း)
```
- ဒီနေရာမှာ max() လို function တွေသုံးရင် Axis သတ်မှတ်ပုံကို သဘောပေါက်ဖို့ အရေးကြီးပါတယ်။ ကျွန်တော်တို့ရဲ့ Array က 2 rows x 3 columns ရှိတဲ့ 2D array ပါ။
- axis = 0 လို့ ပြောလိုက်ရင် "Column အလိုက်ကြည့်မယ်"၊ "Row အလိုက်ကြည့်မယ်" ဆိုပြီး ကျက်မှတ်ထားတာထက် "Collapsing" (ချုံ့ပစ်လိုက်တာ/ဖျောက်လိုက်တာ) ဆိုတဲ့ သဘောတရားနဲ့ မှတ်တာ ပိုမှန်ပါတယ်။
- ဆိုလိုတာက axis = 0 သုံးလိုက်ရင် NumPy က ပထမ Dimension (Size 2 ရှိတဲ့ Row အထပ်လိုက်သဘောတရား) ကို ချုံ့ပစ်လိုက်ပါတယ်။ ဒါကြောင့် ရလဒ်က ကျန်ခဲ့တဲ့ Size 3 အတိုင်း Element ၃ လုံးပါတဲ့ [4,5,6] ဆိုပြီး ထွက်လာတာပါ။
- ဒီသဘောတရားအတိုင်းပဲ axis = 1 သုံးလိုက်ရင် ဒုတိယ Dimension (Size 3 ရှိတဲ့ Column ရေပြင်ညီသဘောတရား) ကို ချုံ့ပစ်လိုက်တဲ့အတွက် [3,6] ဆိုပြီး ရလာတာဖြစ်ပါတယ်။

### 27.4.3 Linear Algebra Operations 
**[English]**
- Note the difference between the two multiplication operations:
```python 
a3 = a1 * a2            # multiplies corresponding elements of a1 and a2
a3 = a1 @ a2            # performs matrix multiplication
a4 = a1.dot(a2)         # performs matrix multiplication
```
- Transpose of a matrix can also be obtained:
```python
a1 = np.array([[1,2,,3,4],[5,6,7,8]])
a2 = np.transpose(a1)
```
- Trace of a matrix is the sum of its diagonal elements. It can be obtained as shown below.
```python
a = np.array([[1,2,3],[4,5,6],[7,8,9]])
s = np.trace(a)         # stores 1 + 5 + 9 = 15
```
- Inverse of a matrix ia a matrix which when multiplied with the original matrix results in an identity matrix. 
```python
a = np.array([[1,2],[3,4]])
b = np.linalg.inv(a)
```
- We can also obtain a solution to linear simultaneous equations. For example, the solution to a system of equations $$ 3x + y = 9 $$ $$and$$ $$ x = 2y = 8 $$ can be obtained as shown below. 
```python 
a = np.array([[3,1],[1,2]])
b = np.array([9,8])
x = np.linalg.solve(a,b)
print(x)
```
**Linear Algebra Operations**

**[Myanmar]**

- NumPy မှာ မြှောက်လဒ်ရှာတဲ့ Operation နှစ်ခုရဲ့ ကွာခြားချက်ကို သတိထားမှတ်သားဖို့ လိုပါတယ်။* ကိုသုံးရင် နေရာတူတဲ့ ကိန်းဂဏန်းချင်း (Element-wise) မြှောက်တာဖြစ်ပြီး၊@ ဒါမှမဟုတ် .dot() ကိုသုံးမှသာ တကယ့် Matrix မြှောက်ခြင်း (Matrix Multiplication) ကို လုပ်ဆောင်တာ ဖြစ်ပါတယ်။
```Python
a3 = a1 * a2            # နေရာတူတဲ့ element အချင်းချင်း မြှောက်ခြင်း (Element-wise)
a3 = a1 @ a2            # Matrix မြှောက်နည်းအတိုင်း မြှောက်ခြင်း (Matrix multiplication)
a4 = a1.dot(a2)         # ဒါကလည်း Matrix multiplication ပါပဲ
```
- Matrix တစ်ခုကို Transpose လုပ်ချင်တယ် (Row နဲ့ Column ပြောင်းပြန်လှန်ချင်တယ်) ဆိုရင်လည်း အလွယ်တကူ လုပ်လို့ရပါတယ်။
```Python
a1 = np.array([[1,2,3,4],[5,6,7,8]])
a2 = np.transpose(a1)
```
- Trace ဆိုတာက Matrix တစ်ခုရဲ့ ထောင့်ဖြတ်မျဉ်း (Principal diagonal) ပေါ်မှာရှိတဲ့ element တွေကို ပေါင်းခြင်းဖြစ်ပါတယ်။ ဒါကို np.trace() နဲ့ ရှာနိုင်ပါတယ်။
```Python
a = np.array([[1,2,3],[4,5,6],[7,8,9]])
s = np.trace(a)         # 1 + 5 + 9 = 15 ဆိုပြီး ရလာပါမယ်
```
- Inverse Matrix ဆိုတာက မူရင်း Matrix နဲ့ ပြန်မြှောက်လိုက်ရင် Identity Matrix ရလာမယ့် Matrix အမျိုးအစားကို ပြောတာပါ။ NumPy ရဲ့ linalg (Linear Algebra) module အောက်က inv() ကိုသုံးပြီး ရှာနိုင်ပါတယ်။
```Python
a = np.array([[1,2],[3,4]])
b = np.linalg.inv(a)
```
- Linear Simultaneous Equations (တစ်ပြိုင်နက်ညီမျှခြင်း) တွေကို ဖြေရှင်းတဲ့နေရာမှာလည်း NumPy ကို သုံးနိုင်ပါတယ်။ဥပမာ - $$3x + y = 9$$ $$နဲ့$$ $$x + 2y = 8$$ ဆိုတဲ့ ညီမျှခြင်းနှစ်ကြောင်းရဲ့ အဖြေကို လိုချင်ရင် အခုလို တွက်နိုင်ပါတယ်။
```Python
a = np.array([[3,1],[1,2]]) # x နဲ့ y ရဲ့ မြှောက်ဖော်ကိန်း (Coefficients) များ
b = np.array([9,8])         # ညီမျှခြင်းရဲ့ ရလဒ်များ
x = np.linalg.solve(a,b)    # အဖြေရှာခြင်း
print(x)
```

### 27.4.4 Bitwise Operations

**[English]**

- Bitwise operations can also be performed on array elements as shown below:
```python 
import numpy as np

a1 = np.array([[10,2,3,4],[5,6,7,8]])
a2 = np.array([[1,1,1,1],[2,2,2,2]])
a3 = np.bitwise_and(a1,a2)
a4 = np.bitwise_or(a1,a2)
a5 = np.bitwise_xor(a1,a2)
a6 = invert(a1)
a7 = np.left_shift(a1,3)               # shifts each element 3 bits to left
a8 = np.right_shift(a1,2)              # shifts each element 2 bits to right
```
**Bitwise Operations**

**[Myanmar]**

- Array ထဲမှာရှိတဲ့ element တစ်လုံးချင်းစီအပေါ်မှာ Bitwise operations တွေကိုလည်း အောက်ပါအတိုင်း တွက်ချက်လုပ်ဆောင်နိုင်ပါသေးတယ်။

```Python

import numpy as np

a1 = np.array([[10,2,3,4],[5,6,7,8]])
a2 = np.array([[1,1,1,1],[2,2,2,2]])

# Bitwise AND, OR, XOR တွက်ချက်ခြင်းများ
a3 = np.bitwise_and(a1,a2)
a4 = np.bitwise_or(a1,a2)
a5 = np.bitwise_xor(a1,a2)

# Invert (NOT) လုပ်ခြင်း
a6 = np.invert(a1)

# Bit Shifting လုပ်ခြင်း
a7 = np.left_shift(a1,3)    # element တစ်ခုစီကို ဘယ်ဘက်သို့ 3 bits ရွှေ့ခြင်း
a8 = np.right_shift(a1,2)   # element တစ်ခုစီကို ညာဘက်သို့ 2 bits ရွှေ့ခြင်း
```

### 27.4.5 Copying and Sorting

**[English]**

- There 3 possible copy operations - no copy, shallow copy operation and deep-copy.
- In no copy, neither the object nor its data gets copied. Only address of array is assigned to a variable. In shallow copy a new array object is created but it points to the same data as the old array object. In deep copy a new array object and copies old object's attributes and data in it.
```python
import numpy as np
a = np.array([[3,3,7],[1,5,2]])
b = a                               # no copy
print(b is a)                       # prints True, a and b are referring to same array
b[0][0] = 100                       # changes a[0][0]

c = a.view()
print(c is a)                       # prints false, a and c are referring to diff objectts
c[0][0] = 50                        # prints [[3 3 7][1 5 2]]
print(d is a)                       # prints False d, a are referring to diff objects
d[0][0] = 150                       # doesn't change a[0][0]

a = np.array([[3,7,6],[1,5,2]])
b = np.array([[3,7,6],[1,5,2]]) 
a.sort()
b.sort(axis = 0)                    # sort elements in each column
```
**Copying and Sorting (ကူးယူခြင်းနှင့် အစီအစဉ်ချခြင်း)**

**[Myanmar]**

- NumPy မှာ Copy ကူးတဲ့နည်းလမ်း (၃) မျိုး ရှိပါတယ်။

    - No Copy: လုံးဝ Copy မကူးခြင်း (Reference သဘောမျိုး)။

    - Shallow Copy (View): အပေါ်ယံ အခွံပဲ ကူးယူခြင်း (Data က အတူတူပဲ)။

    - Deep Copy: အနှစ်ပါမကျန် တစ်စုံလုံး ပွားယူခြင်း။

- No Copy: Object ကိုရော၊ Data ကိုရော ကူးယူတာ မဟုတ်ပါဘူး။ Array ရှိနေတဲ့ လိပ်စာ (Address) ကို Variable အသစ်တစ်ခုနဲ့ လှမ်းညွှန်းလိုက်တာမျိုးပဲ ဖြစ်ပါတယ်။

- Shallow Copy (View): Array object အသစ်တစ်ခု ဖန်တီးလိုက်ပေမယ့်၊ အတွင်းက Data တွေကတော့ မူရင်း Array ရဲ့ Data တွေကိုပဲ မျှသုံးနေတာ (Point လုပ်နေတာ) ဖြစ်ပါတယ်။

- Deep Copy: Array object အသစ်ရော၊ Data အသစ်ရော သီးသန့်ခွဲထုတ်ပြီး အကုန် ကူးယူလိုက်တာ ဖြစ်ပါတယ်။

အောက်ပါ Code ဥပမာမှာ d နဲ့ပတ်သက်တဲ့ အပိုင်း ကျန်ခဲ့လို့ ကျွန်တော် ဖြည့်စွက်ပြီး ရှင်းပြပေးထားပါတယ်ခင်ဗျာ။
```Python

import numpy as np
a = np.array([[3,3,7],[1,5,2]])

# --- No Copy (Reference) ---
b = a                           # Copy ကူးတာမဟုတ်ပါ၊ နာမည်နောက်တစ်ခု တပ်လိုက်တာပါ
print(b is a)                   # True (a နဲ့ b က အတူတူပါပဲ)
b[0][0] = 100                   # b ကို ပြင်လိုက်ရင် a ပါ လိုက်ပြောင်းသွားမယ်

# --- Shallow Copy (View) ---
c = a.view()                    # View အနေနဲ့ ဖန်တီးလိုက်တာပါ
print(c is a)                   # False (Object ချင်း မတူတော့ပါဘူး)
c[0][0] = 50                    # ဒါပေမယ့် c ကို ပြင်ရင် မူရင်း a မှာပါ လိုက်ပြောင်းသွားပါလိမ့်မယ်

# --- Deep Copy ---
d = a.copy()                    # (မူရင်းစာမှာ ဒီ line ကျန်ခဲ့လို့ ဖြည့်ထားပါတယ်)
print(d is a)                   # False (လုံးဝမဆိုင်တဲ့ Object တွေပါ)
d[0][0] = 150                   # d ကို ပြင်လိုက်ရင် မူရင်း a မှာ လိုက်မပြောင်းတော့ပါဘူး
Sorting (အစီအစဉ်ချခြင်း) အတွက်လည်း အောက်ပါအတိုင်း လုပ်ဆောင်နိုင်ပါတယ်။
```
```Python
a = np.array([[3,7,6],[1,5,2]])
b = np.array([[3,7,6],[1,5,2]]) 

a.sort()                # Row အလိုက် ငယ်စဉ်ကြီးလိုက် စီပေးသွားမယ်
b.sort(axis = 0)        # Column အလိုက် (ဒေါင်လိုက်) ငယ်စဉ်ကြီးလိုက် စီပေးသွားမယ်
```

### 27.4.6 Comparison 

**[English]**

- Three types of comparsions are common with arrays:
    - (a) Compare all elements of an array witth one value and return a Boolean array of the result. 
    - (b) Compare corresponding elements of two arrays and return an array of Booleans. 
    - (c) Compare shape and elements of two array, return TRUE if equl, FALS other wise. 
- Comparsion of all array elements with one value:
```python
import numpy as np
a = np.array([[3,7,6],[1,5,2]])
print(a < 5)                # prints [[Ture False False][True False True]]
```
- Comparison of corresponding array elements:
```python
import numpy as np
a = np.array([[3,7,6],[1,5,2]])
b = np.array([[3,1,2],[1,7,2]])
print(a < b)                # prints [[False False False][False True False]]
```
- Comparison of two arrays:
```python
import numpy as np
a = np.array([[3,7,6],[1,5,2]])
b = np.array([[3,7,6],[1,5,2]])
c = np.array([[3,7],[6,1],[5,2]])
print(np.array_equal(a,b))  # True, Shape & Elements Match
print(np.array_equal(a,c))  # False, different shapes
```
**Comparison (နှိုင်းယှဉ်ခြင်းများ)**

**[Myanmar]**

- Array တွေမှာ ယှဉ်ကြည့်စရာ၊ တိုက်စစ်စရာ (Comparison) ပုံစံ (၃) မျိုး ရှိပါတယ်။

    - (a) One Value Comparison: Array ထဲက Element အားလုံးကို တန်ဖိုးတစ်ခုတည်းနဲ့ လိုက်ယှဉ်ကြည့်ပြီး ရလာတဲ့ အဖြေ (True/False) ကို Array ပြန်ထုတ်ပေးတာ။
    - (b) Corresponding Elements Comparison: Array နှစ်ခုမှာရှိတဲ့ နေရာတူ Element အချင်းချင်း လိုက်ယှဉ်ကြည့်ပြီး Boolean Array ပြန်ထုတ်ပေးတာ။
    - (c) Full Array Comparison: Array နှစ်ခုရဲ့ ပုံသဏ္ဍာန် (Shape) ရော၊ ပါဝင်တဲ့ Element တွေရော ထပ်တူညီမညီ စစ်ဆေးတာ (တူရင် True, မတူရင် False ပြပါတယ်)။

- (1) Array Element အားလုံးကို တန်ဖိုးတစ်ခုနဲ့ လိုက်ယှဉ်ခြင်း
```Python
import numpy as np
a = np.array([[3,7,6],[1,5,2]])
print(a < 5)                # 5 ထက်ငယ်လား လိုက်စစ်တာပါ
# အဖြေက [[True False False] [True False True]] ဆိုပြီး ထွက်ပါမယ်
```
- (2) Array နှစ်ခုက နေရာတူ Element အချင်းချင်း ယှဉ်ခြင်း
```Python
import numpy as np
a = np.array([[3,7,6],[1,5,2]])
b = np.array([[3,1,2],[1,7,2]])
print(a < b)                # a က b ထက် ငယ်သလား နေရာတူချင်း တိုက်စစ်တာပါ
# အဖြေက [[False False False] [False True False]] ဆိုပြီး ထွက်ပါမယ်
```
- (3) Array နှစ်ခုလုံး ထပ်တူညီမညီ ယှဉ်ခြင်း
```Python
import numpy as np
a = np.array([[3,7,6],[1,5,2]])
b = np.array([[3,7,6],[1,5,2]])
c = np.array([[3,7],[6,1],[5,2]])

print(np.array_equal(a,b))  # True (Shape ရော Element တွေရော ကွက်တိတူလို့ပါ)
print(np.array_equal(a,c))  # False (Shape မတူတော့လို့ပါ)
```

### 27.4.7 Indexing and Slicing

**[English]**

- As with lists, single element indexing is 0-based and accepts negative indices for indexing from end of the array. 
```python
a = np.array([3,7,6,1,5,2])
print(a[0],a[-1])           # prints 3 2
```
- Individual elements of a mutli-dimensional array are accessed using multiple indices.
```python
a = np.array([[3,7,6],[1,5,9]])
print(a[1][2])              # prints 9 9
```
- Note that in **a[1][2]**, a new temporary array is created after first index (i.e. [1,5,9]) and then its second element is fetched. 
- Slicing works same as lists except that it can be applied to multiple dimensions. 
```python
import numpy as np
a = np.array([8,2,4,1,5,9])
b = np.array([[3,7,6,9,8],[1,5,9,2,4]])
print(a[2:5])               # prints [4 1 5]
pirnt(a[:-4])               # prints [8 2]
print(b[1:3,2:4])           # prints [[9 2][3 1]]
print(b[1:3][2:4])          # prints []
```
- Note that in **b[1:3][2:4]** firstly arrays[[1,5,9,2,4][0,0,3,1,5]] is created and then elements 2 to 3 are fetched from it. Since this new array has only two elements, it returns [].

**Indexing and Slicing (Array ခန်းများ ညွှန်းဆိုခြင်းနှင့် အပိုင်းဖြတ်ခြင်း)**

**[Myanmar]**

- Python List တွေလိုပါပဲ၊ NumPy Array တွေကလည်း 0 ကနေစပြီး ရေတွက် (Indexing လုပ်) ပါတယ်။ အနောက်ဆုံးကနေ ပြန်ရေချင်ရင် အနုတ်လက္ခဏာ (Negative index) သုံးလို့ရပါတယ်။
```Python
a = np.array([3,7,6,1,5,2])
print(a[0], a[-1])          # 3 နဲ့ 2 ကို ထုတ်ပေးပါလိမ့်မယ် (ရှေ့ဆုံးနဲ့ နောက်ဆုံး)
```
- Dimension တစ်ခုထက်ပိုတဲ့ Array (Multi-dimensional array) တွေမှာ အခန်းတစ်ခန်းချင်းစီကို လှမ်းယူချင်ရင် Index နံပါတ်တစ်ခုမက သုံးရပါတယ်။

```Python

a = np.array([[3,7,6],[1,5,9]])
print(a[1][2])              # 9 ကို ထုတ်ပေးပါလိမ့်မယ်
# (a[1] က ဒုတိယမြောက် Row [1,5,9] ဖြစ်ပြီး၊ အဲ့ဒီထဲက index 2 ဖြစ်တဲ့ 9 ကို ယူလိုက်တာပါ)
```
- သတိပြုရန် - a[1][2] လို့ရေးတာက ကွန်ပျူတာအလုပ်လုပ်ပုံအရ နည်းနည်းကွာခြားပါတယ်။ သူက ပထမ a[1] အပိုင်းကို အရင်ဆွဲထုတ်ပြီး ယာယီ array (temporary array) တစ်ခုအရင်ဆောက်လိုက်တယ်၊ ပြီးမှ အဲ့ဒီအထဲက index 2 ကို ထပ်ဆွဲထုတ်တာ ဖြစ်ပါတယ်။ (NumPy မှာ ပိုမြန်ချင်ရင် a[1, 2] လို့ရေးတာက ပိုကောင်းပါတယ်)။

- Slicing (အပိုင်းဖြတ်တာ) ကလည်း List တွေအတိုင်းပါပဲ။ ထူးခြားတာက Dimension တွေအများကြီးမှာ ကော်မာ (comma) ခံပြီး တပြိုင်နက် ဖြတ်လို့ရတာပါပဲ။

```Python

import numpy as np
a = np.array([8,2,4,1,5,9])
# b မှာ မူရင်းစာသားအရ Row 3 ကြောင်းရှိမယ်လို့ ယူဆရပါတယ် (ရှင်းလင်းချက်အရ)
b = np.array([[3,7,6,9,8], [1,5,9,2,4], [0,0,3,1,5]]) 

print(a[2:5])               # [4 1 5] (Index 2 ကနေ 5 မတိုင်ခင်ထိ)
print(a[:-4])               # [8 2] (အစကနေ နောက်ဆုံး 4 လုံးမတိုင်ခင်ထိ)

# 2D Slicing (Comma သုံးထားပုံကို သတိပြုပါ)
print(b[1:3, 2:4])          
# Row 1 ကနေ 3 မတိုင်ခင်ထိ (Row 1, 2) ယူမယ်၊ 
# Column 2 ကနေ 4 မတိုင်ခင်ထိ (Col 2, 3) ယူမယ်။
# ရလဒ်က [[9 2], [3 1]] ဆိုပြီး ထွက်ပါမယ်။
```
- အရေးကြီးတဲ့ အချက် (Common Mistake)

- b[1:3][2:4] လို့ရေးတာနဲ့ b[1:3, 2:4] လို့ရေးတာ မတူပါဘူး။

- b[1:3][2:4] လို့ရေးလိုက်ရင် ပထမ b[1:3] အရ Row 1 နဲ့ 2 ပါတဲ့ Array အသစ်တစ်ခု ထွက်လာမယ်။ ပြီးတော့မှ အဲ့ဒီ Array အသစ်ရဲ့ Row 2 ကနေ 4 ကို ထပ်ဖြတ်ဖို့ ကြိုးစားပါလိမ့်မယ်။ Array အသစ်မှာက Row 2 row ပဲရှိတော့ [2:4] ဆိုတဲ့ row တွေ မရှိတော့ပါဘူး။ ဒါကြောင့် အဖြေက Empty Array [ ] (အလွတ်) ထွက်လာတာ ဖြစ်ပါတယ်။

## 27.5 Array Manipulation

**[English]**

- Once an array is created we can change its shape using the method **reshape()**. This method returns an array ccontaining same data, but a new shape. 
```python
import numpy as np
a = np.array([[3,7,6,9],[0,3,1,5]])
b = a.reshape(2,6)
print(b)                        # prints[[3 7 6 9 1 5][2 4 0 3 1 5]]
c = a.reshape(4,-1)
print(c)                        # prints [[3 7 6][9 1 5][2 4 0][3 1 5]]
d = np.arange(12).reshape(2,6)  
print(d)                        # prints [[0 1 2 3 4 5][6 7 8 9 10 11]]
```
- We can faltten a multi-dimensional array.
```python
import numpy as np
a = np.array([[3, 7, 6, 9],[1, 5, 2, 4],[0, 3, 1,, 5]])
b = a.ravel()
print(b)                        # prints [3 7 6 9 1 5 2 4 0 3 1 5]
```
- We can append values at the end of an existing array. 
```python
import numpy as np
a = np.array([[3, 7, 6, 9],[1, 5, 2, 4]])
b = np.array([[0, 3, 1, 5],[1, 1, 1, 1]])
c = np.append(a,b,axis=0)
d = np.append(a,b,axis=1)
print(c)                # prints[[3 7 6 9][1 5 2 4][0 3 1 5][1 1 1 1]]
print(d)                # prints[[3 7 6 9 0 3 1 5][1 5 2 4 1 1 1 1]]
```
- Note that the values are appended to a copy of existing array. The values being appended must be of same shape as existing array. If *axis* is not specified, *values* can be any shape and will be flattened before use. 
- There exist functions that let you insert elements, delete elements, split array etc. You are advised to expore them on your own.


**Array Manipulation (Array များကို ပုံစံပြောင်းလဲ ကိုင်တွယ်ခြင်း)**

**[Myanmar]**

- Reshaping (ပုံသဏ္ဍာန် ပြောင်းလဲခြင်း) Array တစ်ခုကို တည်ဆောက်ပြီးပြီဆိုရင် reshape() method ကိုသုံးပြီး သူ့ရဲ့ ပုံသဏ္ဍာန် (Shape) ကို ပြောင်းလဲနိုင်ပါတယ်။ ဒီ Method က Data တွေကို မထိခိုက်စေဘဲ Shape အသစ်နဲ့ Array တစ်ခုကို ပြန်ထုတ်ပေးတာပါ။

*(မှတ်ချက် - မူရင်းစာသားပါ Code တွင် Element အရေအတွက် ကွဲလွဲမှုရှိနေသဖြင့် တွက်ချက်၍ရအောင် အနည်းငယ် ပြင်ဆင်ရှင်းပြပေးထားပါတယ်)*

```Python

import numpy as np
# Element ၁၂ လုံးပါတဲ့ Array တစ်ခု (3 rows x 4 columns)
a = np.array([[3,7,6,9],[1,5,2,4],[0,3,1,5]]) 

# 2 rows x 6 columns ပုံစံ ပြောင်းမယ်
b = a.reshape(2,6)
print(b)
# ရလဒ်: [[3 7 6 9 1 5] [2 4 0 3 1 5]]

# Row 4 ကြောင်းလိုချင်တယ်၊ Column ကိုတော့ Auto တွက်ထည့်စေချင်ရင် '-1' သုံးရတယ်
c = a.reshape(4,-1)
print(c)
# ရလဒ်: [[3 7 6] [9 1 5] [2 4 0] [3 1 5]] (4 rows x 3 columns ဖြစ်သွားမယ်)

# 0-11 အထိ ဂဏန်းတွေကိုထုတ်ပြီး တန်းပြီး reshape လုပ်ခြင်း
d = np.arange(12).reshape(2,6)  
print(d)                        
# ရလဒ်: [[0 1 2 3 4 5] [6 7 8 9 10 11]]
```
- Flattening (ပြားချခြင်း) Multi-dimensional array (အထပ်ထပ်ပါတဲ့ array) တစ်ခုကို ravel() သုံးပြီး 1D array (တန်းတစ်တန်းတည်းဖြစ်သွားအောင်) ပြားချလိုက်လို့ ရပါတယ်။
```Python

import numpy as np
a = np.array([[3, 7, 6, 9],[1, 5, 2, 4],[0, 3, 1, 5]])
b = a.ravel()
print(b)                        
# ရလဒ်: [3 7 6 9 1 5 2 4 0 3 1 5] ဆိုပြီး တစ်တန်းတည်း ထွက်လာမယ်
```
- Appending (ထပ်ဖြည့်ခြင်း) ရှိပြီးသား Array တစ်ခုရဲ့ အနောက်မှာ နောက်ထပ် တန်ဖိုးတွေ ထပ်ဖြည့်ချင်ရင် np.append() ကို သုံးနိုင်ပါတယ်။
```Python

import numpy as np
a = np.array([[3, 7, 6, 9],[1, 5, 2, 4]])
b = np.array([[0, 3, 1, 5],[1, 1, 1, 1]])

# Axis 0 (Row အလိုက်/အောက်ဘက်သို့) ဆက်မယ်
c = np.append(a, b, axis=0)
# ရလဒ်: Row ၄ ကြောင်း ဖြစ်လာမယ်

# Axis 1 (Column အလိုက်/ဘေးဘက်သို့) ဆက်မယ်
d = np.append(a, b, axis=1)
# ရလဒ်: Row 2 ကြောင်းပဲ ရှိမယ်၊ ဒါပေမယ့် Column တွေ များသွားမယ်
```
**သတိပြုရန် -**

- append လုပ်လိုက်ရင် မူရင်း Array ကို သွားပြင်တာမဟုတ်ဘဲ၊ တန်ဖိုးသစ်တွေပါဝင်တဲ့ Array အသစ်တစ်ခု (Copy) ကို ထုတ်ပေးတာ ဖြစ်ပါတယ်။ ထပ်ဖြည့်မယ့် Array ဟာ မူရင်း Array နဲ့ Shape တူညီဖို့ လိုပါတယ်။ တကယ်လို့ axis မသတ်မှတ်ထားဘူးဆိုရင် Array တွေကို အရင်ဆုံး ပြားချ (Flatten) လိုက်ပြီးမှ ဆက်ပေးသွားမှာ ဖြစ်ပါတယ်။ 
- ဒါ့အပြင် Array တွေထဲမှာ Element ကြားဖြတ်ထည့်တာ (Insert)၊ ဖျက်တာ (Delete) နဲ့ ခွဲထုတ်တာ (Split) လုပ်တဲ့ Function တွေလည်း ရှိပါသေးတယ်။ ဒါတွေကိုတော့ ကိုယ့်ဘာသာ ဆက်လက်လေ့လာကြည့်ဖို့ အကြံပြုထားပါတယ်။
---

## Problems


### Problem 27.1
- Write a program that constructs a 3D array of dimensions 4 x 2 x 3. Initialize the array to some values. Find the maximum along each axis.

<details>
<summary><b>Program</b></summary>

```python 
import numpy as np
a = np.array([[[3,7,6],[1,5,2]],[[1,2,4],[7,2,9]],[[1,0,0],[5,4,3]],[[8,1,4],[2,7,8]]])
print('Maximum along axis 0')
print(np.max(a,axis = 0))
print('Maximum along axis 1')
print(np.max(a,axis = 1))
print('Maximum along axis 2')
print(np.max(a,axis = 2))
```
</details>

<details>
<summary><b>Output</b></summary>

```python
Maximum along axis 0
[[8 7 6]
[7 7 9]]
Maximum along axis 1
[[3 7 6]
[7 2 9]
[5 4 3]
[8 7 8]]
Maximum along axis 2 
[[7 5]
[4 9]
[1 5]
[8 8]]
```
</details>

### Problem 27.2 
- Write a program to create an array of shape 5 x 4 containing elements 1 to 20. Find the sum of entire array as well as sums along each row and column. 

<details>
<summary><b>Program</b></summary>

```python
import numpy as np
a = np.arange(20).reshape((5,4))
print(a)
print(np.sum(a))
print(np.sum(a, axis = 0))
print(np.sum(a, axis = 1))
```
</details>

<details>
<summary><b>Output</b></summary>

```python
[[0 1 2 3]
[4 5 6 7]
[8 9 10 11]
[12 13 14 15]
[16 17 18 19]]
190
[40 45 50 55]
[6 22 38 54 70]
```
</details>



### Problem 27.3
- Write a program to achieve the following tasks:
    - Create an array *a* of size 10 with each element of it set to a value 3.
    - Find the memory size of this array and its individual element.
    - Create an array *b* of size 10 with values ranging from 0 to 90 evenly spaced.
    - Reverse elements of array *b*.
    - Add arrays *a* and *b* and store the result in array *c*.

<details>
<summary><b>Program</b></summary>

```python
import numpy as np
a = np.full(10,3)
print(a)
print(a.nbytes)
print(a.itemsize)
b = np.linspace(0,90,10)
print(b)
b = b[::-1]
print(b)
c = a + b
print(c)
```
</details>

<details>
<summary><b>Output</b></summary>

```python
[3 3 3 3 3 3 3 3 3 3]
40
4
[0. 10. 20. 30. 40. 50. 60. 70. 80. 90.]
[90. 80. 70. 60. 50. 40. 30. 20. 10. 0.]
[93. 83. 73. 63. 53. 43. 33. 23. 13. 3.]
```
</details>

### Problem 27.4

- Write a program to achieve the following tasks:
    - Create a 2D array of size 5 x 5 with elements on border set to 1, and all inner elements set to *a* value 3. 
    - Multiply a 4 x 3 matrix containing all 2s.
    - Given a 1D array, negate all elements which are between 2 and 8, in place. 

<details>
<summary><b>Program</b></summary>

```python
import numpy as np
a = np.ones((5,5))
print(a)
b = np.ones((4,3))
c = np.full((3,5),2)
d = b @ c
print(d)
e = np.arange(11)
print(e)
e[(2 < e) & (e < 8)] *= -1
print(e)
```
</details>

<details>
<summary><b>Output</b></summary>

```python 
[[1. 1. 1. 1. 1.]
[1. 3. 3. 3. 1.]
[1. 3. 3. 3. 1.]
[1. 3. 3. 3. 1.]
[1. 1. 1. 1. 1.]]
[[6. 6. 6. 6. 6.]
[6. 6. 6. 6. 6.]
[6. 6. 6. 6. 6.]
[6. 6. 6. 6. 6.]]
[0 1 2 3 4 5 6 7 8 9 10]
[0 1 2 -3 -4 -5 -6 -7 8 9 10]
```
</details>

## Exercises

<details>
<summary>Extercises</summary>

- [A] State whether the following statements are True or False:
    - [ ] Numpy library gets installed when we install Python.
    - [ ] Numpy arrays work faster than lists.
    - [ ] Numpy array elements can be of different types.
    - [ ] Once created, a Numpy arrays size and shape can be changed dynmically.
    - [ ] **np.array_equal(a,b)** would return **True** if shape and elements of *a* and *b* match. 

- [B] Answer the following questions: 
    - (a) How will you create Numpy Array of first 10 natural numbers? 
    - (b) Can we create an array of complex numbers using Numpy?
    - (c) How would you create 5 arrays each of size 3 x 4 x 5 and fill them with values, 0, 1,5, random and garbage values respectively? 
    - (d) How would you create a 50-element array and fill it with odd numbers starting from 1? 
    - (e) How will you obtain the type of elements, number of elements, base address and number of bytes occupied by the following Numpy array? 
    - (f) How will you obtain dimension and shape of a Numpy array created by **a1 = np.array([[1,2,3,4],[5,6,7,8]])**?
    - (g) Given two 3 x 4 matrices how would you add, subtract, multiply and divide corresponding elements of these matrices? 
    - (h) Which of the following are the scalar arithmetic operations on Numpy array?
    
    ```python
    a1 = np.array([[10,2,3,4],[5,6,7,8]]) 
    a2 = np.array([[1,1,1,1],[2,2,2,2]])
    a3 = a1 + a2
    a4 = a1 - a2
    a5 = a1 * a2
    a6 = a1 / a2
    a7 = a1 % a2
    a8 = a1 ** 2
    a9 += a1
    a10 += 5
    a11 = a1 + 2
    a12 = a1 ** 2
    ```
- [C] Match The Following pairs:

| Code / Function | Operation / Description |
| :--- | :--- |
| (a) `s = np.trace(a)` | 1. Statistical Operation |
| (b) `s = a.cumsum(axis = 1)` | 2. Linear Algebra Operation |
| (c) `a2 = np.copy(a1)` | 3. Deep copy operation |
| (d) `print(a1 < 2)` | 4. Corresponding ele.comparison |
| (e) `print(a1 > a2)` | 5. Comparison with one value |
| (f) `print(a[1:3][3:6])` | 6. Bitwise Operation |
| (g) `a2 = invert(a1)` | 7. Slicing Operation |
 
 </details>




