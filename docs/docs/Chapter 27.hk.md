CHAPTER 27

# Numpy Library

## Table of Contents (A Chung Ummi Pawl)
- [Keynote (Biapi)](#keynote-biapi)
- [27.1 Creation of Array (Array Sernak)](#271-creation-of-array-array-sernak)
- [27.2 Creation of Filler Arrays (A Chung Thil Um Cia Array Sernak)](#272-creation-of-filler-arrays-a-chung-thil-um-cia-array-sernak)
- [27.3 Array Attributes (Array Sining)](#273-array-attributes-array-sining)
- [27.4 Array Operations (Array Tuahnak Pawl)](#274-array-operations-array-tuahnak-pawl)
  - [27.4.1 Arithmetic Operations (Kanan Tuahnak)](#2741-arithmetic-operations-kanan-tuahnak)
  - [27.4.2 Statistical Operations (Statistic Tuahnak)](#2742-statistical-operations-statistic-tuahnak)
  - [27.4.3 Linear Algebra Operations (Linear Algebra Tuahnak)](#2743-linear-algebra-operations-linear-algebra-tuahnak)
  - [27.4.4 Bitwise Operations (Bitwise Tuahnak)](#2744-bitwise-operations-bitwise-tuahnak)
  - [27.4.5 Copying and Sorting (Copy Tuah le Remh)](#2745-copying-and-sorting-copy-tuah-le-remh)
  - [27.4.6 Comparison (Tahchunhnak)](#2746-comparison-tahchunhnak)
  - [27.4.7 Indexing and Slicing (Index Tuah le Hleh)](#2747-indexing-and-slicing-index-tuah-le-hleh)
- [27.5 Array Manipulation (Array Sersiamnak)](#275-array-manipulation-array-sersiamnak)
- [Problems (Harnak/Tuahding)](#problems-harnaktuahding)
- [Exercises (Lentecelhnak)](#exercises-lentecelhnak)

---

## Keynote (Biapi)

- Numpy cu Numerical Python tinak a si. Hi library hi science le engineering lei buaibainak phitnak ah hman a si. Hi nih hin a ttha mi multidimensional array object, le array cung ah rian rang tein tuah khawhnak lam a kan pek. Hi rian tuahnak ah mathematical, logical, shape manipulation, sorting, selecting, I/O, statistical operations, le a dangdang an i tel.

---

## 27.1 Creation of Array (Array Sernak)

- **Numpy Library** hman na duh ah cun, download le install na tuah a hau, a tanglei bantuk in:
```bash
pip install numpy
```
- Numpy Array cu Python list he an i lo ngai nain, lists nakin a rian a rang deuh.
- List he aa lo lo nak cu, Numpy array chung i element (thil) vialte kha an type (phun) aa khat dih a hau.
- Numpy array ser na duh ah cun np.array() function na hman a hau i, a chung ah number list kha na pek a hau, a tanglei bantuk in:
```python
import numpy as np
intarr = np.array([1,2,3,4]) # integer (nambar tling) array a ser
floattarr = np.array([1.1,2.2,3.3,4.4]) # float (nambar cheu) array a ser
```
- 2D array (matrix) cu 1D arrays tampi fonhmi a si i, 3D array cu 2D arrays tampi fonhmi a si. A tanglei bantuk in ser khawh an si:
```python
a1 = np.array([[1,2,3],[4,5,6]]) # rows 2 x column 3
a2 = np.array([[[1,2],[4,5]],[[6,7],[8,9]]]) # 2,2 x 2 arrays
```
- Complex numbers array zong ser khawh a si:
```python
c = np.array([[1,2],[3,4]],complex)
```
---

## 27.2 Creation of Filler Arrays (A Chung Thil Um Cia Array Sernak)
- Numpy Arrays cu a hramthawk ah thil (values) a um cia mi in kan ser khawh, a hnu ah thlen khawh a si.
- Tahchunhnak ah, a chung ah 0s lawng a um mi, 1s lawng a um mi, asiloah a dang value a um mi kan ser khawh. A chung ah garbage values (sullam a ngei lo mi nambar) a um mi empty arrays zong kan ser khawh.
```python
import numpy as np
a1 = np.empty((3,4))  # 2D array garbage values he a ser
a2 = np.zeros((3,4))  # 2D array zeros he a ser
a3 = np.ones((3,4))   # 2D array ones he a ser
a4 = np.full((2,2),7) # 2D array a chung ummi 7 he a ser
```             
- Hi functions hna sin ah tuples pek a hau. Tuples (3,4) le (2,2) nih array kan ser ding mi a shape (pungsan/size) a chim.
- Random values (nambar sawhsawh) asiloah aa khat te in a then mi values he array kan ser khawh.
```python
import numpy as np
a1 = np.random.random((4))  # 4 random values he a ser
a2 = np.arange(5)            # [0,1,2,3,4]
a3 = np.linspace(0,2,5)     # [0.0 0.5 1.0 1.5 2.0]
```
- arange() le linspace() i a hmasa parameter pahnih cu a thawknak le a donghnak values an si. arange() i a pathumnak parameter cu step value (karh zat) a si, linspace() i a pathumnak parameter cu kan ser duh mi values zat a si.
- Numpy nih identity matrix sernak nawl a kan pek, mah cu principal diagonal ah ones a um i, a dang vialte zeros a um mi matrix a si.
```python
import numpy as np
a1 = np.eye(3)
a2 = np.identity(3)
```
- Identity matrix cu square matrix a si caah dimension 1 lawng eye() le identity() ah pek a hau.

---

## 27.3 Array Attributes (Array Sining)
- Numpy array nih attributes tampi a ngei i, cu nih element type, element size, array shape, array size, tbk. a langhter.
- Numpy array chung i elements type, an size, le memory ah an umnak hmun tbk. kan hmu khawh.
```python
import numpy as np
a1 = np.array([1,2,3,4])
a2 = np.array([1.1,2.2,3.3,4.4])
print(a1.dtype)                 # int32 a print
print(a2.dtype)                 # float64 a print
print(a1.itemsize)              # 4 a print
print(a2.itemsize)              # 8 a print
print(a1.nbytes)                # 16 a print
print(a2.nbytes)                # 16 a print
print(a1.data)                  # <memory at 0x024BEE08> a print
print(a1.strides)               # (4,) a print
print(a2.data)                  # <memory at 0x0291EE08> a print
print(a2.strides)               # (8,) a print
```
- Hika ah dtype nih array chung i elements type a langhter. itemsize nih array element pakhat i bytes a lak zat a langhter i, nbytes nih array dihlak i bytes a lak zat a langhter.
- data nih memory ah array a umnak hmun (base address) a langhter i, strides nih a hnu i array element phanhnak ding ah base address ah bytes zeizat dah chap a hau ti a langhter.
- ndim, shape le size attributes nih array i dimensions zat, array shape le a chung i elements zat a langhter.

```python
import numpy as np
a1 = np.array ([1,2,3,4])
a2 = np.array(([1,2,3,4],[5,6,7,8]))
print(a1.ndim)                       # 1 a print
print(a2.ndim)                       # 2 a print
print(a1.shape)                      # tuple (4,) a print
print(a2.shape)                      # tuple (2,4) a print
print(a1.size)                       # 4 a print
print(a2.size)                       # 8 a print
```
- ndim nih array dimensions zat, shape nih array shape zat, size nih array size zat a langhter.

---
## 27.4 Array Operations (Array Tuahnak Pawl)
- Numpy arrays cung ah operations (tuahnak) tampi tuah khawh a si. Hi operations hna cu a tawi i a rang. Library chung ah precompiled routines a um cia mi hman a si caah a rang.
- Array operations a phunphun hna cu:
    (a) Arithmetic Operations (Kanan Tuahnak)
    (b) Statistical Operations (Statistic Tuahnak)
    (c) Linear Algebra Operations (Linear Algebra Tuahnak)
    (d) Bitwise Operations (Bitwise Tuahnak)
    (e) Copying, Sorting (Copy Tuah le Remh)
    (f) Comparsion Operations (Tahchunhnak Tuah)

### 27.4.1 Arithmetic Operations (Kanan Tuahnak)
- Array pahnih cung ah **+, -, *, /, %** tbk. operations na tuah khawh. Hi operators na hman tikah, array pahnih i a zawn cio elements cung ah operations kha a tuah. Hi operators hman lo in, **add()**, **subtract()**, **multiply()**, **divide()**, le **remainder()** methods zong na hman khawh. Hi operations hna cu vector operations tiah auh a si tawn.
```python
import numpy as np
a1 = np.array([[10,2,3,4],[5,6,7,8]])
a2 = np.array([[1,1,1,1],[2,2,2,2]])
a3 = a1 + a2                            # a3 = np.add(a1,a2) he aa khat
a4 = a1 - a2
a5 = a1 * a2
a6 = a1 / a2
a7 = a1 % a2
a8 = a1 ** 2                            # element kip kha power 2 in a kaiter
```
- a1 le a2 le array pahnih i a zawn cio elements cung ah operations kha a tuah.
- a3 le a4 le a5 le a6 le a7 le a8 le array pahnih i a zawn cio elements cung ah operations kha a tuah.
- a8 le array pahnih i a zawn cio elements cung ah operations kha a tuah.
- Array elements cung ah scalar arithmetic operations kan tuah khawh. Hi operations hna cu elementwise operations tiah auh a si tawn.

```python
import numpy as np
a1 = np.array([[10,2,3,4],[5,6,7,8]])
a2 = a1 + 2             # element kip ah 2 a chap
a3 = a1 **2             # element kip kha power 2 in a kaiter
```
- In place operators +=, -=, /= nih array thar ser lo in a um cia mi array kha a thlen.
```python
a1 += a2 # a1 = a1 + a2 he aa khat
a3 += 5  # a3 = a3 + 5 he aa khat
```
Array elements cung ah a dang operations tuah khawh mi hna cu exp(), sqrt(), cos(), sin(), log().

### 27.4.2 Statistical Operations (Statistic Tuahnak)
- Numpy nih a tanglei operations hna hi array elements dihlak cung ah asiloah axis (dimension) a chimh mi elements cung ah a tuah khawh. Note: Axis cu dimension tinak a si, cucaah 1D array nih axis 1 a ngei, 2D array nih axis 2 a ngei.
```python
import numpy as np
a = np.array([[1,2,3,],[4,5,6]])
print(a.sum())
print(a.min())                      # array chung i a hme bik a kawl
print(a.max(axis = 0))              # column (tung) kip i a ngan bik a kawl
print(a.max(axis = 1))              # row (phei) kip i a ngan bik a kawl
print(a.sum(axis = 1))              # axis 1 lei ah a fonh
print(a.cumsum(axis = 1))           # cumulative sum
print(np.mean(a))
print(np.median(a))
print(np.corrcoef(a))
print(np.std(a))
```
- **sum()** nih array chung i a hme bik a kawl, **min()** nih array chung i a hme bik a kawl, **max()** nih array chung i a hme bik a kawl, **max()** nih array chung i a hme bik a kawl, **sum()** nih array chung i a hme bik a kawl, **cumsum()** nih array chung i a hme bik a kawl, **mean()** nih array chung i a hme bik a kawl, **median()** nih array chung i a hme bik a kawl, **corrcoef()** nih array chung i a hme bik a kawl, **std()** nih array chung i a hme bik a kawl.
- **max()** kan hman tikah axis hman ning theih hi a biapi. Kan array cu 2D array a si i dimensions 2 x 3 a ngei. axis = 0 kan hman tikah, 'column lei max' asiloah 'row lei max' tiah ruat hlah. A sullam cu axis = 0 kan hman tikah, Numpy nih size 2 kha a thumh (condense), cu tikah result cu elements 3 [4,5,6] a ngei mi array a si. Cu bantuk in, axis = 1 kan hman tikah, Numpy nih size 3 kha a thumh, cu tikah result cu elements [3,6] a ngei mi array a si.

### 27.4.3 Linear Algebra Operations (Linear Algebra Tuahnak)
- Multiplication operations pahnih i dannak kha theih a hau:
```python
a3 = a1 * a2            # a1 le a2 i a zawn cio elements a multiply (karh)
a3 = a1 @ a2            # matrix multiplication a tuah
a4 = a1.dot(a2)         # matrix multiplication a tuah
```
- Matrix i transpose zong kan hmu khawh:
```python
a1 = np.array([[1,2,3,4],[5,6,7,8]])
a2 = np.transpose(a1)
```
- Matrix i trace cu a diagonal elements i a sum a si. A tanglei bantuk in hmuh khawh a si.
```python
a = np.array([[1,2,3],[4,5,6],[7,8,9]])
s = np.trace(a)         # 1 + 5 + 9 = 15 a khon
```
- Matrix i inverse cu a matrix i a inverse a si. A tanglei bantuk in hmuh khawh a si.
```python
a = np.array([[1,2,3],[4,5,6],[7,8,9]])
a_inv = np.linalg.inv(a)
```
- Linear simultaneous equations i phitnak (solution) zong kan hmu khawh. Tahchunhnak ah, equations system $$3x + y = 9$$ $$le \\  x + 2y = 8$$ i phitnak cu a tanglei bantuk in hmuh khawh a si.
```python
a = np.array([[3,1],[1,2]])
b = np.array([9,8])
x = np.linalg.solve(a,b)
print(x)
```
- Eigenvalues and eigenvectors cu a matrix i a eigenvalues and eigenvectors a si. A tanglei bantuk in hmuh khawh a si.
```python
a = np.array([[1,2],[3,4]])
eigvals, eigvecs = np.linalg.eig(a)
print(eigvals)
print(eigvecs)
```
### 27.4.4 Bitwise Operations (Bitwise Tuahnak)
- Array elements cung ah Bitwise operations zong a tanglei bantuk in tuah khawh a si:
```python
import numpy as np

a1 = np.array([[10,2,3,4],[5,6,7,8]])
a2 = np.array([[1,1,1,1],[2,2,2,2]])
a3 = np.bitwise_and(a1,a2)
a4 = np.bitwise_or(a1,a2)
a5 = np.bitwise_xor(a1,a2)
a6 = np.invert(a1)
a7 = np.left_shift(a1,3)               # element kip bits 3 in keilei ah a shift
a8 = np.right_shift(a1,2)              # element kip bits 2 in orhlei ah a shift
```
### 27.4.5 Copying and Sorting (Copy Tuah le Remh)
- Copy operations phun 3 a um - no copy (copy lo), shallow copy (a leng copy) le deep-copy (a thuuk copy).
- No copy ah, object asiloah a data kha copy a si lo. Array umnak address lawng variable ah pek a si. Shallow copy ah array object thar a ser nain data hlun kha a hman. Deep copy ah array object thar a ser i attributes le data hlun kha a copy dih.
```python
import numpy as np
a = np.array([[3,3,7],[1,5,2]])
b = a                               # no copy
print(b is a)                       # True a print, a le b cu array pakhat ah an i kawk
b[0][0] = 100                       # a[0][0] a thleng

c = a.view()
print(c is a)                       # false a print, a le c cu object dangdang an si
c[0][0] = 50                        # [[3 3 7][1 5 2]] a print
d = a.copy()
print(d is a)                       # False a print, d le a cu object dangdang an si
d[0][0] = 150                       # a[0][0] a thleng lo

a = np.array([[3,7,6],[1,5,2]])
b = np.array([[3,7,6],[1,5,2]])
a.sort()
b.sort(axis = 0)                    # column (tung) kip i elements a sort
```
- Array sorting phun 2 a um - in place sorting (copy lo) le out of place sorting (copy lo).
### 27.4.6 Comparison (Tahchunhnak)
- Arrays he tahchunhnak phun 3 hman tawn a si:
    - (a) Array elements dihlak kha value pakhat he tahchunh i Boolean array result chuah.
    - (b) Array pahnih i a zawn cio elements tahchunh i Booleans array chuah.
    - (c) Array pahnih i shape le elements tahchunh, aa khah ah cun TRUE, aa khah lo ah cun FALSE.
- Array elements dihlak value pakhat he tahchunhnak:
```python
import numpy as np
a = np.array([[3,7,6],[1,5,2]])
print(a < 5)                # [[True False False][True False True]] a print
```
- Array pahnih i a zawn cio elements tahchunhnak:   
```python
import numpy as np
a = np.array([[3,7,6],[1,5,2]])
print(a < 5)                # [[True False False][True False True]] a print
```
- Array pahnih i a zawn cio elements tahchunhnak:   
```python
import numpy as np
a = np.array([[3,7,6],[1,5,2]])
b = np.array([[3,1,2],[1,7,2]])
print(a < b)                # [[False False False][False True False]] a print
```
- Array pahnih i shape le elements tahchunhnak:
```python
import numpy as np
a = np.array([[3,7,6],[1,5,2]])
b = np.array([[3,1,2],[1,7,2]])
print(a < b)                # [[False False False][False True False]] a print
```

```python
import numpy as np
a = np.array([[3,7,6],[1,5,2]])
b = np.array([[3,7,6],[1,5,2]])
c = np.array([[3,7],[6,1],[5,2]])
print(np.array_equal(a,b))  # True, Shape & Elements Aa Khat
print(np.array_equal(a,c))  # False, shape aa dang
```

### 27.4.7 Indexing and Slicing (Index Tuah le Hleh)
- Lists bantuk in, element pakhat indexing cu 0 in a thok i array a donghnak in indexing tuah duh ah negative indices (nambar) a cohlan.
```python
a = np.array([3,7,6,1,5,2])
print(a[0],a[-1])           # 3 2 a print
```
- Mutli-dimensional array i element pakhat kha indices tampi hman in lak khawh a si.
```python
a = np.array([[3,7,6],[1,5,9]])
print(a[1][2])              # 9 9 a print
```
- Note: a[1][2] ah, index hmasa (i.e. [1,5,9]) hnu ah temporary array thar a ser i, cun a chung i a pahnihnak element kha a lak.
- Slicing cu lists he aa lo nain dimensions tampi ah hman khawh a si.
```python
import numpy as np
a = np.array([8,2,4,1,5,9])
b = np.array([[3,7,6,9,8],[1,5,9,2,4]])
print(a[2:5])               # [4 1 5] a print
print(a[:-4])               # [8 2] a print
print(b[1:3,2:4])           # [[9 2][3 1]] a print
print(b[1:3][2:4])          # [] a print
```
- Note: **b[1:3][2:4]** ah, hmasa ah **arrays[[1,5,9,2,4][0,0,3,1,5]]** a ser i, cun elements 2 in 3 tiang a lak. Hi array thar cu elements pahnih lawng a ngeih caah, [] a chuah.

---
## 27.5 Array Manipulation (Array Sersiamnak)
- Array ser a si hnu ah reshape() method hmang in a shape (pungsan) kan thlen khawh. Hi method nih data cu aa khat nain shape thar a ngei mi array a chuah.
```python
import numpy as np
a = np.array([[3,7,6,9],[0,3,1,5]])
b = a.reshape(2,6)
print(b)                        # [[3 7 6 9 1 5][2 4 0 3 1 5]] a print
c = a.reshape(4,-1)
print(c)                        # [[3 7 6][9 1 5][2 4 0][3 1 5]] a print
d = np.arange(12).reshape(2,6)
print(d)                        # [[0 1 2 3 4 5][6 7 8 9 10 11]] a print
```
- Multi-dimensional array cu kan flatten (a perter) khawh.
```python
import numpy as np
a = np.array([[3, 7, 6, 9],[1, 5, 2, 4],[0, 3, 1, 5]])
b = a.ravel()
print(b)                        # [3 7 6 9 1 5 2 4 0 3 1 5] a print
```
- A um cia mi array a donghnak ah values kan append (chap) khawh.
```python
import numpy as np
a = np.array([[3, 7, 6, 9],[1, 5, 2, 4]])
b = np.array([[0, 3, 1, 5],[1, 1, 1, 1]])
c = np.append(a,b,axis=0)
d = np.append(a,b,axis=1)
print(c)                # [[3 7 6 9][1 5 2 4][0 3 1 5][1 1 1 1]] a print
print(d)                # [[3 7 6 9 0 3 1 5][1 5 2 4 1 1 1 1]] a print
```
- Note: Values cu a um cia mi array i a copy ah chap a si. Chap ding mi values cu a um cia mi array he shape aa khat a hau. axis chimh a si lo ah cun, values cu shape zeipaoh a si kho i hman hlan ah flatten tuah a si lai.

- Elements insert tuahnak, delete tuahnak, split tuahnak tbk functions an um. Nangmah te in hlathlai ding in forh na si.

---

## Problems (Harnak/Tuahding)
### Problem 27.1
- Dimensions 4 x 2 x 3 a ngei mi 3D array sernak program tial. Values cheukhat in initialize (hramthawk) tuah. Axis kip i a maximum (ngan bik) kawl. 

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
#Maximum along axis 0
[[8 7 6]
[7 7 9]]
#Maximum along axis 1
[[3 7 6]
[7 2 9]
[5 4 3]
[8 7 8]]
#Maximum along axis 2
[[7 5]
[4 9]
[1 5]
[8 8]]
```
</details>
---
### Problem 27.2
- Shape 5 x 4 a ngei mi le elements 1 in 20 tiang a ngei mi array sernak program tial. Array dihlak i sum (fonh), row le column kip i sum kawl.
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
- A tanglei rian hna tuahnak ding ah program tial: 
    - Size 10 a ngei mi array a ser, a chung i element kip value 3 ah chiah. 
    - Hi array le a chung i element pakhat i memory size kawl. 
    - Size 10 a ngei mi array b ser, a chung i values cu 0 in 90 tiang aa khat te in a then mi si seh. - Array b i elements kha a let (reverse) in tuah. 
    - Array a le b fonh law a result kha array c ah khon.

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
<details><summary><b>Output</b></summary>

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
- A tanglei rian hna tuahnak ding ah program tial:
    - Size 5 x 5 a ngei mi 2D array ser, a border (rim) i elements kha 1 ah chiah, a chung elements vialte value 3 ah chiah.
    - 4 x 3 matrix, a chung ah 2s lawng a um mi he multiply tuah.
    - 1D array pakhat pek a si tikah, 2 le 8 karlak a um mi elements vialte kha negate (minus ah thlen), in place in tuah.
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
<details><summary><b>Output</b></summary>

```python
[[1. 1. 1. 1. 1.]
[1. 3. 3. 3. 1.]
[1. 3. 3. 3. 1.]
[1. 3. 3. 3. 1.]
[1. 1. 1. 1. 1.]
[[6. 6. 6. 6. 6.]
[6. 6. 6. 6. 6.]
[6. 6. 6. 6. 6.]
[6. 6. 6. 6. 6.]]
[0 1 2 3 4 5 6 7 8 9 10]
[0 1 2 -3 -4 -5 -6 -7 8 9 10]
```
</details>
---

# Exercises (Lentecelhnak)
<details>
<summary>Exercises</summary>
- [A] A tanglei statements hi True (Hmaan) maw False (Hmaan lo) ti chim:
    - [ ] Python kan install tikah Numpy library zong aa install chih.
    - [ ] Numpy arrays cu lists nakin a rian a rang deuh.
    - [ ] Numpy array elements cu types (phun) aa dang mi a si kho.
    - [ ] Array ser a si hnu ah, a size le shape cu dynamically in thlen khawh a si.
    - [ ] a le b i shape le elements an i khah ah cun np.array_equal(a,b) nih True a return lai.

- [B] A tanglei biahalnak hna hi phi:
    - [ ] First 10 natural numbers i Numpy Array zeitin dah na ser lai?
    - [ ] Numpy hmang in complex numbers array kan ser kho maw?
    - [ ] Size 3 x 4 x 5 a ngei mi arrays 5 kha zeitin dah na ser lai i, a values cu 0, 1, 5, random le garbage values cio in na khahter lai?
    - [ ] 50-element array zeitin dah na ser lai i, 1 in a thok mi odd numbers (nambar tial) in na khahter lai?
    - [ ] A tanglei Numpy array i elements type, elements zat, base address le bytes a lak zat zeitin dah na hmuh lai?
    - [ ] **a1 = np.array([[1,2,3,4],[5,6,7,8]])** in ser mi Numpy array i dimension le shape zeitin dah na hmuh lai?
    - [ ] 3 x 4 matrices pahnih pek a si tikah, hi matrices i corresponding elements kha zeitin dah add, subtract, multiply le divide na tuah hna lai?
    - [ ] A tanglei hna lakah khuazei hi dah Numpy array cung i scalar arithmetic operations an si?
    
    ```Python 
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
- [C] A tanglei pairs hna hi a match (aa tlak) mi thim:

| Code / Function | Operation / Description|
| :--- | :--- |
|(a) `s = np.trace(a)` | 1. Statistical Operation|
|(b) `s = a.cumsum(axis = 1)`| 2. Linear Algebra Operation|
|(c) `a2 = np.copy(a1)` |3. Deep copy operation|
|(d) `print(a1 < 2)`| 4.     Corresponding ele.comparison|
|(e) `print(a1 > a2)` | 5. Comparison with one value|
|(f) `print(a[1:3][3:6])`| 6. Bitwise Operation|
|(g) `a2 = invert(a1)`| 7. Slicing Operation|

</details>