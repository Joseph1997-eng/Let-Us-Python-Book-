# Chapter 3 Python Basics

<div class="chapter-social-card">
  <div class="chapter-info">
    <div class="chapter-number">CHAPTER 3</div>
    <h1 class="chapter-title">Python Basics</h1>
  </div>
  <div class="chapter-logo">
    <img src="/Let-Us-Python-Book-/Logo.png" alt="Joseph Logo">
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

### 3.1 **Identifiers** Le **Keywords**

**Python** cu **case sensitive** (ca ngan le ca hme a thleidan mi) **language** a si. **Python identifier** cu **variable**, **function**, **class**, **module**, asiloah **object** dang hngalh/thleidan nak caah hman mi min a si.

**Identifiers** ser nak phunglam pawl:

* **Alphabet** (ca) asiloah **underscore** (_) in aa thawk a hau.

* A hnu ah **letters**, **_**, le **digits** (nambar) an zul kho.

* **keyword** cu **identifier** in hman khawh a si lo.

**Keywords** dihlak cu **lowercase** (ca hme) in an si (Note: **False**, **None** le **True** ti lo). **Python** nih *Table 3.1* ah hmuh sak mi **keywords** **33** a ngei.

|Table 3.1 Keywords list| | | |
|---|---|---|---|
|False|continue|from|not|
|None|def|global|or|
|True|del|if|pass|
|and|elif|import|raise|
|as|else|in|return|
|assert|except|is|try|
|break|finally|lambda|while|
|class|for|nonlocal|with|
|yield|

A tanglei **statements** hmang in **Python keywords** list kha na **print** khawh:

```python title="checking keyword list"
import keyword # makes the module 'keyword' available
print(keyword.kwlist) # syntax modulename.object/function
```

---

### 3.2 **Python** Types

**Python** nih **data types** phun 3 a **support**:

* **Basic Types**:
    * **int**, **float**, **complex**, **bool**, **string**, **bytes**
* **Container Types**:
    * **list**, **tuple**, **set**, **dict**
* **User-defined types**:
    * **class**

Hi hna lak ah, **basic types** kong cu hi **chapter** ah a tling tein fianh a si lai. **Container types** kong cu a tawi nak in fianh a si lai. **Container type** pakhat cio caah a dang tein **chapter** ser a si, cuka ah cun a tling tein fianh a si lai. **User-defined types** cu hi **chapter** ah fianh a si lai lo. **Chapter 17** ah zeitin dah ser le hman ding an si ti kha fianh a si.



---

#### 3.2.1 Basic Types

**Basic types** aa dangdang hna i tahchunhnak cu a tanglei ah pek an si:

* **int** cu **binary**, **decimal**, **octal**, **hexadecimal** in langhter khawh a si.
* **binary** cu **0b/0B** in aa thawk, **octal** cu **0o/0O** in, **hex** cu **0x/0X** in aa thawk (tahchunhnak: 0b10111, 156, 0o432, 0x4A3).
* **float** cu **fractional** asiloah **exponential form** in langhter khawh a si (tahchunhnak: 314.1528, 3.141528e2, 3.141528E2).
* **complex** ah **real** le **imaginary part** an um (tahchunhnak: 3 + 2j, 1 + 4J).
* **bool** cu **Boolean values** pahnih lak ah pakhat paoh a si kho i an pahnih in ca lian in an i thawk (tahchunhnak: **True**, **False**).
* **string** cu **Unicode characters** a hlawm a si i thlen khawh a si lo (**immutable**), `' '`, `" "`, asiloah `""" """` chung ah chiah a si. 'Rosanna', "Rosanna", """Rosanna""".
* **bytes** nih **binary data** a aiawh.

```python title="bytes example"
b'\xa1\xe4\x56' # hex values a1a456 a ngei mi bytes 3 a aiawh
```
Data pakhat i a type kha **type()** tiah auh mi function hmang in chek khawh a si, a tanglei bantuk in:

```python title="checking type of data using type() function"
print(type(35)) # <class 'int'> tiah a print/langhter
print(type(3.14)) # <class 'float'> tiah a print/langhter
```

#### 3.2.2 Integer Le Float Ranges

* **int** cu a duh zahzah a ngan a si kho (limit a um lo).

```python title="integer example"
a = 123
b = 1234567890
c = 123456789012345678901234567890
```
**Python** nih **arbitrary precision integers** a ngei. Cucaah na duh zah a ngan mi **integers** na ser khawh. Cun, **integers** cung ah **arithmetic operations** (tuaknak) na tuah tik ah **overflow/underflow** (limit luan/tlhum lo) kong ah lungretheih a hau lo.

**Floats** cu computer chung ah **IEEE 754 standard** ning in **64-bit double-precision values** in **binary** ah chiah/langhter an si. Hi **standard** ning in cun, **float** nih a ngeih khawh mi a ngan bik value cu **1.8 x 10^308** hrawng a si. Hi nak in a ngan mi nambar cu **inf** (short for **infinity** - tawpnak ngei lo) in langhter a si.

**Floats** tampi cu **binary form** in 'a dik thlap in' (**exactly**) langhter khawh an si lo. Cucaah a chung i chiah ning (**internal representation**) cu a taktak value he 'aa lo nawn' (**approximation**) in chiah a si tawn.

A taktak **value** le an langhter mi **value** i an i dannak cu a hme tuk, cucaah buaibainak nganpi a chuahter tawn lo.

### 3.3 **Variable Type** Le **Assignment**

**Variable** i a **type** kha khiah/chimh cia a hau lo. **Execution** a tuah lio ah **variable** i a **type** cu zeitin dah hman a si timi **context** zoh in amah tein a lak (**inferred**). Cucaah **Python** cu **dynamically-typed language** tiah auh a si.

```python title="Variable type"
a = 25 # a i type cu int tiah a lak/hngalh
a = 31.4 # a i type cu float tiah a lak/hngalh
a = 'Hi' # a i type cu str tiah a lak/hngalh
```

**Variable** pakhat i a type kha **type()** timi **built-in function** hmang in chek khawh a si.

```python title="str variable"
a = 'Job Kaa'
print(type(a)) # type cu str tiah a report/langhter lai
```

A fawi mi **variable assignment** (value pek ning):

```python title="assignment example"
a = 10
pi = 3.14
name = 'Rosanna'
```

**Variables** tampi a voikhat ah **assignment** tuah ning (value pek ning):

```python title="multiple assignment example"
a = 10 ; pi = 31.4 ; name = 'Rosanna' # ; hi statement separator in hman a si
a, pi, name = 10, 3.14, 'Rosanna'
a = b = c = d = 5
```

#### 3.3.1 **Arithmetic Operators**

Arithmetic Operators: **`+, - , * , /, %, //, **`**

```python title="Arithmetic Operators"
a = 4 / 2 # true division a tuah i float 2.0 a chuah
a = 7 % 2 # % nih a taang mi (remainder) 1 a chuah
b = 3 ** 4 # ** nih 3 a voi 4 nak a chuah (exponentiation)
c = 4 // 3 # // nih fractional part (a cheu) hlawt in quotient 1 a chuah
```

**In-place assignment operators** nih **arithmetic operations** (tuaknak) caah **shortcut** (lam tawi) ṭha taktak a pek. Cu hna cu **`+=, -=, *=, /=, %=, //=, **=`** an si.

```python title="In-place assignment"
a **= 3 # a = a ** 3 he aa khat
b %= 10 # b = b % 10 he aa khat
```

### 3.3.2 **Operation Nuances** (Tuaknak I A Sining Pawl)

**Floor division** `a//b` kan tuah tik ah, a chuak mi **result** (a phi) cu **quotient** (a cheu mi a phi taktak) nak in a niam deuh mi asiloah aa khat mi **integer** (nambar tling) a ngan bik kha a si. **//** cu **floor division operator** tiah an auh.

(Note: Negative nambar a um tik ah a niam lei/thlang lei ah a kal. Tahchunhnak ah `-10` kha `3` in cheu ah `-3.33` a si, asinain **floor division** nih cun `-3.33` nak in a niam deuh mi `-4` tu a laak).

```python title="Floor Division"
print(10 // 3) # 3 a chuah
print(-10 // 3) # -4 a chuah
print(10 // -3) # -4 a chuah
print(-10 // -3) # 3 a chuah
print(3 // 10) # 0 a chuah
print(3 // -10) # -1 a chuah
print(-3 // 10) # -1 a chuah
print(-3 // -10) # 0 a chuah
```

**-10 // 3** ah, **-10** hmuh ding in **3** i a let cu **-3.333** a si, a **floor value** cu **-4** a si.
**10 // -3** ah, **10** hmuh ding in **-3** i a let cu **-3.333** a si, a **floor value** cu **-4** a si.
**-10 // -3** ah, **-10** hmuh ding in **-3** i a let cu **3.333** a si, a **floor value** cu **3** a si.

**print( )** cu **function** a si i screen cung ah **output** langhter ding ah hman a si. Lam phunphun in hman khawh a si. Cu hna cu **Chapter 7** ah fianh a si lai.

**a % b** timi operation cu **a - (b * (a // b))** tiah tuak a si. Hihi a tanglei tahchunhnak pawl hman hian fawi tein hngalh khawh a si:

```python title="print functions"
print(10 % 3) # 1 a chuah
print(-10 % 3) # 2 a chuah
print(10 % -3) # -2 a chuah
print(-10 % -3) # -1 a chuah
print(3 % 10) # 3 a chuah
print(3 % -10) # -7 a chuah
print(-3 % 10) # 7 a chuah
print(-3 % -10) # -3 a chuah
```

**`a % b`** cu `a - (b * (a // b))` tiah tuak a si caah, **`-10 % 3`** cu `-10 - (3 * (-10 // 3))` tiah tuak a si i, **2** a chuak. **`10 % -3`** cu `10 - (-3 * (10 // -3))` tiah tuak a si i, **-2** a chuak. **`-10 % -3`** cu `-10 - (-3 * (-10 // -3))` tiah tuak a si i, **-1** a chuak.

Mathematical rule *`a / b x c`* le *`a x c / b`* hi an i khat tawn, asinain a zungzal in a si lo (Computer chung ah cun).

```python title="Mathematical rule"
# a tanglei expressions hna hi an result (a phi) aa khat
a = 300 / 100 * 250
a = 300 * 250 / 100

# Asinain, a tanglei hna hi cu an i khat lo
b = 1e210 / 1e200 * 1e250
b = 1e210 * 1e250 / 1e200 # INF (tawpnak ngei lo) a chuak
```

**True** cu `1` a si i **False** cu `0` a si caah, an pahnih in belh (add) khawh an si.

```python title="True and False"
a = True + True # 2 a chuah
b = True + False # 1 a chuah
```

### 3.4 **Precedence** Le **Associativity**

**Arithmetic expression** pakhat chung ah **operators** tampi hman an si tik ah, hman mi **operators** pawl i an **precedence** (**priority** - biapi ah chiah in tuak hmasa ding) cung ah hngat in tuak a si.

**Priority** a sang bik in a niam bik lei **operators** pawl (**PEMDAS**):

```python title="Precedence of operators"
( ) # Parentheses (Kuek)
** # Exponentiation (A let)
*, /, //, % # Multiplication, Division (Tuk, Cheu)
+, - # Addition, Subtraction (Belh, Thwn)
```

**Precedence** (priority) aa khat mi **operators** pahnih an um a si ahcun, **associativity** hmang in biakhiahnak tuah a si (aho dah tuah hmasa ding ti kha).

**Operator** pakhat cio nih **left to right associativity** (Keh lei in Orh lei) asiloah **right to left associativity** (Orh lei in Keh lei) an ngei.

Tahchunhnak ah `c = a * b / c` ah, `*` kha `/` nak in tuah hmasa a si, a ruang cu **arithmetic operators** nih **left to right associativity** an ngeih caah a si (Keh lei in a rat tik ah `*` nih a hmuh hmasa).

**Python operators** dihlak, an **priority** le an **associativity** cazin tling cu **Appendix A** ah pek a si.

#### 3.4.1 **Conversions** (Thlen Ning)

**Mixed mode operations** (Cawh-nuk in tuahnak):

* **int** le **float** karlak ah tuah a si ahcun **float** a chuak.
* **int** le **complex** karlak ah tuah a si ahcun **complex** a chuak.
* **float** le **complex** karlak ah tuah a si ahcun **complex** a chuak.

**Numeric type** pakhat in a dang pakhat ah thlen ding caah **int( )**, **float( )**, **complex( )** le **bool( )** timi **built-in functions** hna hi hman khawh an si.

**Type conversions:**

```python title="Type conversions"
int(float/numeric string) # float asiloah numeric string in int ah thlen
int(numeric string, base) # numeric string kha base a um mi int ah thlen
float(int/numeric string) # int asiloah numeric string in float ah thlen
float(int) # int in float ah thlen
complex(int/float) # complex ah thlen (imaginary part 0 in)
complex(int/float, int/float) # complex ah thlen (real le imaginary he)
bool(int/float) # int/float in True/False (1/0) ah thlen
str(int/float/bool) # string ah thlen
chr(int) # int he aa tlak mi character (ca) ah thlen
```

**int( )** nih a cheu mi (quotient) i a point hnu (decimal portion) kha a hlonh, cucaah zero lei ah a **round** (a tling mi ah a thlen) zungzal.

```python title="int()"
a = int(3.33) # 3 a chuah
b = int(-3.33) # -3 a chuah
```

#### 3.4.2 **Built-in Functions** (A Chung Um Cia Functions)

**Python** nih **built-in functions** (amah chung ah a um cia mi) tampi a ngei, cu hna cu **program** chung khoika hmun paoh ah hman khawh an si. Screen cung ah **output** langhter ding caah kan hman tawn mi **print( )** function zong kha **built-in function** pakhat a si.

**Built-in function** pakhat paoh kong he pehtlai in bawmhnak (**help**) hmuh na duh ahcun **help(function)** kha hman khawh a si.

Nambar he hman tawn mi **Built-in functions** pawl cu a tanglei ah pek an si:

```python title="Built-in functions"
abs(x) # x i a absolute value (a man taktak) a chuah
pow(x, y) # x a voi y nak (x raised to y) a chuah
min(x1, x2,...) # arguments lak ah a hme bik a chuah
max(x1, x2,...) # arguments lak ah a ngan bik a chuah
divmod(x, y) # (x // y, x % y) kha pair (a kop) in a chuah
round(x [,n]) # point hnu ah n digits um ding in x kha a round
bin(x) # x he aa khat mi binary a chuah
oct(x) # x he aa khat mi octal a chuah
hex(x) # x he aa khat mi hexadecimal a chuah
```

A tanglei **Python program** nih hi **built-in functions** cheukhat hman ning a hmuhsak:

```python title="Built-in functions"
a = abs(-3) # a ah 3 a chiah (assign)
print(min(10, 20, 30, 40)) # 10 a print/langhter
print(hex(26)) # 1a a print/langhter (Python taktak ah cun 0x1a tiah a lang)
```

#### 3.4.3 **Built-in Modules**

**Built-in functions** leng ah, **Python** nih **built-in modules** tampi a pek. **Module** pakhat cio ah **functions** tampi an um.
**Mathematical operations** a sang deuh mi tuah ding caah **built-in modules** a simi **math**, **cmath**, **random**, **decimal** chung i **functions** pawl kha hman khawh an si.

```python title="Built-in modules"
math - hman a ṭhahnem mi mathematics functions tampi.
cmath - complex numbers cung ah operations tuahnak functions.
random - random number (nambar can-u-nan) sernak he aa tlai mi functions.
decimal - arithmetic operations a dik thlap in (precise) tuahnak functions.
```

**math** module chung i **Mathematical functions** pawl:

```python title="Mathematical functions in math module"
pi, e # constants pi le e i an values (man)
sqrt(x) # x i square root
factorial(x) # x i factorial
fabs(x) # float x i absolute value (a man taktak)
log(x) # x i natural log (base e hman in log)
log10(x) # x i base-10 logarithm
exp(x) # e a voi x nak (e raised to x)
trunc(x) # integer ah thlen/tan (point hnu hlonh)
ceil(x) # x nak in a ngan deuh asiloah aa khat mi integer a hme bik
floor(x) # x nak in a niam deuh asiloah aa khat mi integer a ngan bik
modf(x) # x i a fractional (a cheu) le integer parts (a tling) pawl
```

**round( )** timi **built-in function** cu **decimal places** (point hnu) a biaki mi zah tiang **round** tuah khawh a si, asinain **math** module i library functions **trunc( )**, **ceil( )** le **floor( )** pawl nih cun **decimal places** zero (point hnu um lo) tiang lawng an **round** zungzal.

**math** module chung i **Trigonometric functions** pawl:

```python title="Trigonometric functions in math module"
degrees(x) # radians in degrees ah thlen
radians(x) # degrees in radians ah thlen
sin(x) # x radians i sine
cos(x) # x radians i cosine
tan(x) # x radians i tan
sinh(x) # x i hyperbolic sine
cosh(x) # x i hyperbolic cosine
tanh(x) # x i hyperbolic tan
acos(x) # x i cos inverse, radians in
asin(x) # x i sine inverse, radians in
atan(x) # x i tan inverse, radians in
hypot(x, y) # sqrt(x * x + y * y) (Hypotenuse tuaknak)
```

**random** module chung i **Random number generation functions** pawl:

```python title="Random number generation functions from random module"
random( ) # 0 le 1 karlak ah random number (nambar can-u-nan)
randint(start, stop) # start le stop karlak (range) ah random number
seed( ) # random number sernak hram (seed) caah atu lio caan (current time) kha a hman
seed(x) # random number sernak hram (seed) caah x kha a hman
```
**Module** pakhat chung i **functions** pawl hman khawh ding caah, **import** statement hmang in **module** kha **import** (lak) kan tuah a hau.

A tanglei **Python program** nih **math** module le **random** module chung i **functions** cheukhat hman ning a hmuhsak:

```python title="Using functions from math and random modules"
import math
import random
print(math.factorial(5)) # 120 a print/langhter
print(math.degrees(math.pi)) # 180.0 a print/langhter
print(random.random( )) # 0.8960522546341796 a print/langhter
```
**Built-in functions** tampi an um i **built-in module** pakhat cio chung ah **functions** tampi an um fawn. **Functions** pawl i an min philh a fawi te. A tanglei **program** hi hman in a ran nak in kan hmuh/chek khawh hna:

```python title="Getting list of built-in functions"
import math
print(dir(__builtins__)) # builtins hmailei le hnulei ah underscore pahnih cio an um
print(dir(math))
```
### 3.5 **Container Types**

**Container types** tiah chim tik ah a tlangpi in **values** tampi hmun khat ah chiah ṭi kha a chim duh mi a si. **Basic types** aa dangdang hna i tahchunhnak cu a tanglei ah pek an si:

```python title="Container types"
# list cu index in kawl khawh mi, thilri a phunphun chiah ṭi nak a si
[10, 20, 30, 20, 30, 40, 50, 10], ['She', 'sold', 10, 'shells']

# tuple cu thlen khawh lo mi (immutable) hlawm a si
('Rosanna', 34, 4500.55), ('Let Us Python', 350, 195.00)

# set cu values aa dang cio (unique) lawng chiah ṭi nak a si
{10, 20, 30, 40}, {'Rosanna', 34, 45000}

# dict cu key-value pairs hlawm a si, a unique mi key kha '' chung ah chiah a si
{'ME101' : 'Strength of materials', 'EE101' : 'Electronics'}
```
**List** le **tuple** chung i **values** pawl cu an umnak hmun (**position**) hmang in lak khawh an si. **Set** chung i **values** pawl cu **for** loop hmang in lak khawh an si (hihi **Chapter 6** ah fianh a si lai). **Dictionary** chung i **values** pawl cu **key** hmang in lak khawh an si. Hihi a tanglei **program** ah hmuhsak a si:


```python title="Accessing values in container types"
lst = [10, 20, 30, 20, 30, 40, 50, 10]
tpl = ('Let Us Python', 350, 195.00)
s = {10, 20, 30, 40}
dct = {'ME101' : 'SOM', 'EE101' : 'Electronics'}
print(lst[0], tpl[2]) # 10 195.0 a print/langhter
print(dct['ME101']) # SOM a print/langhter
```

#### 3.5.1 **Python Type Jargon** (Biafang Hman Mi Pawl)

**Python types** kong chim tik ah a tanglei biafang pawl hi hman an si tawn:

* **Collection** - **container types** caah hman mi biafang a si.
* **Iterable** - **loop** hman in a chung thil pakhat hnu pakhat kal khawh mi/lanh khawh mi **collection** a si.
* **Ordered collection** - **elements** (a chung thil) kha kan khumh ning tein an um. Cucaah **index** (a umnak hmun) hmang in lak khawh an si.
* **Unordered collection** - **elements** kha kan khumh ning tein an um lo. Cucaah **element** pakhat hi khoika hmun ah dah a um ti kan chim kho lo. Cucaah **position based index** hmang in lak khawh a si lo.
* **Sequence** - **ordered collection** caah hman mi biafang a si.
* **Immutable** - thlen khawh lo mi **collection** (unchangeable).
* **Mutable** - thlen khawh mi **collection** (changeable).

Atu ah cun kan hmuh ciami **types** pawl hi zeibantuk sining dah an ngeih ti zoh hna usih:

* **String** - ordered collection, immutable, iterable.
* **List** - ordered collection, mutable, iterable.
* **Tuple** - ordered collection, immutable, iterable.
* **Set** - unordered collection, mutable, iterable.
* **Dictionary** - unordered collection, mutable, iterable.

#### 3.5.2 **Comments** Le **Indentation**

**Comments** cu **#** in an i thawk.

```python title="Comments begin with #"
# calculate gross salary (gross salary tuaknak)
gs = bs + da + hra + ca 
si = p * n * r / 100 # calculate simple interest (simple interest tuaknak)
```

**Catlang tampi a um mi comments** (Multi-line comments) pawl cu **'''** (triple single quotes) asiloah **"""** (triple double quotes) chung ah ṭial a hau.

```python title="Multi-line comments should be written in a pair of ''' or \"\"\"."
''' Additional program: Calculate bonus to be paid
URL: [https://github.com/Joseph1997-eng/Let-Us-Python-Book-](https://github.com/Joseph1997-eng/Let-Us-Python-Book-) ([https://github.com/Joseph1997-eng/Let-Us-Python-Book-](https://github.com/Joseph1997-eng/Let-Us-Python-Book-))
Author: Joseph, Date: 7 Dec 2025 '''
```

**Indentation** (catlang hram ṭhawn) hi a biapi tuk! Na duh poh in hmang hlah. A tanglei **code** nih **'Unexpected indent'** error a chuahter lai.

```python title="Indentation matters! Don’t use it casually. Following code will report an error 'Unexpected indent'."
a = 20 
  b = 45 # Indentation a herh lo nak hmun ah tuah a si caah Error a piah lai
```

**Multi-lining** (Catlang Tampi In Ṭial)

**Statements** an sau tuk a si ahcun, catlang tampi ah ṭhen in ṭial khawh an si. A tawpnak catlang dah ti lo, a dang catlang donghnak paoh ah **`\`** (backslash) chiah a hau.

```python title="Multi-lining"
total = physics + chemistry + maths + \
english + myanmar + history + \
geography + civics
```
**`[ ]`**, **`{ }`**, asiloah **`( )`** chung ah **statements** kha catlang tampi (**multi-line**) in ṭial a si tik ah **`\`** (backslash) hman a hau lo.

```python title="Multi-line" 
days = [ 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 
'Friday', 'Saturday', 'Sunday' ]
```

### 3.6 **Classes** Le **Objects**

**Python** ah **type** paoh cu **class** an si. Cucaah **int**, **float**, **complex**, **bool**, **str**, **list**, **tuple**, **set**, **dict** pawl hi **classes** an si dih. Hi hna cu hman ding in a um cia mi (**ready-made**) **classes** an si. **Python** nih kanmah tein **class** ser (**user-defined classes**) zong a kan onh, hihi **Chapter 18** ah kan hmuh te lai.

**Object** cu **class** in ser a si. **Class** nih thil pahnih a fianter — cu **class** in ser mi **object** cu zeidah a lawh lai (a sining) le cu **object** laknak le tawlrelnak caah hman khawh mi **methods** (functions) pawl an si.

**Class** pakhat in **objects** tampi ser khawh a si. **Class** in **object** ser a si tik ah, **class** i **instance** ser a si tiah chim a si.

**Class** nih min a ngei, asinain **objects** nih min an ngei lo. **Objects** nih min an ngeih lo caah, memory chung i an umnak **addresses** (hmun) hmang in auh asiloah hngalh an si.

A cunglei chim mi dihlak hi a tanglei **program** hmang hian hneksak/hmuh khawh a si. A sullam ṭha tein hngalh ding in **Observation** (Hmuhning) kha zoh.



```python title="All the above statements can be verified through the following program."
a = 30
b = 'Good'
print(a, b) # 30 Good tiah a print
print(type(a), type(b)) # <class 'int'> <class 'str'> tiah a print
print(id(a), id(b)) # 1356658640 33720000 (Memory address pawl) tiah a print
print(isinstance(a, int), isinstance(b, str)) # True True tiah a print
```

### 3.7 **Python Object Reference Visualization** (Python Object Pawl Hmuhning)

**Python** ah **variables** nih **memory** chung i **objects** an hngaih/lak ning hngalh hi a biapi tuk.


!!! note "Key Concept (A Biapi Mi):"
    * **Python** ah cun, **variables** cu **memory** chung i a um mi **objects** a kawhhmuhtu **references** (asiloah **pointers**) an si. **Values** (a man) kha anmah chung ah an chiah lo, value umnak **memory location** (hmun) tu kha an kawk.

## **Memory Reference Breakdown**

A tanglei **table** nih diagram chung i **references** pawl kha a tial:

| Variable Name | Reference ID (Address) | Points To (Object Type) | Object Value | Object Memory Address |
| :--- | :--- | :--- | :--- | :--- |
| **`a`** | `1356658640` | **int object** | `30` | `1356658640` |
| **`b`** | `33720000` | **str object** | `Good` | `33720000` |


!!! note "Observation (Hmuhning):"
    * **Variable `a`** nih reference ID `1356658640` a ngei, cucu **Integer Object** `30` i a **address** he aa khat.
    * **Variable `b`** nih reference ID `33720000` a ngei, cucu **String Object** `'Good'` i a **address** he aa khat.

Hi **program** chung ah **objects** pahnih kan ser — pakhat cu **ready-made class** a simi **int** in le a dang pakhat cu **ready-made class** a simi **str** in kan ser.

**int** type object nih `30` a ngei, cun **str** type object nih `'Good'` a ngei.

**Object** pahnih hna hi min an ngei lo. **Memory** chung i an **addresses** `1356658640` le `33720000` kha `a` le `b` chung ah chiah an si.

Hi **addresses** pawl cu **built-in function** a simi **id( )** hmang in hmuh khawh an si. **Program** na **execute** (tuahter) tik ah **addresses** aa dang na hmuh kho men (computer aa dan ah aa dang kho).

`a` le `b` nih **addresses** an ngeih caah, cu **addresses** ah a um mi **objects** kha an **refer** (kawk/hngaih) tiah chim a si. A fawi nak in chim ahcun **objects** a kawktu **pointers** an si.

`a` le `b` nih an **refer** mi **objects** i an **type** kha **built-in function** a simi **type( )** hmang in hmuh khawh a si.

`a` hi **class int** i **instance** a si le si lo kha **built-in function** a simi **isinstance( )** hmang in chek khawh a si.

**Multiple Objects**

A tanglei **program** hi zoh hmanh:

```python title="Multiple Objects"
a = 3
b = 3
print(id(a), id(b)) # 1356658640 1356658640 tiah a print (an id aa khat)
print(a is b) # True tiah a print (object khat an si caah)

a = 30 # atu ah cun a nih object dang a refer cang
print(id(a)) # 1356659072 (address thar) tiah a print
```

**int** object pahnih kan ser maw? A si lo. **int** object chung i um mi value (3) aa khat mi a si caah, **int** object 1 lawng ser a si. `a` le `b` nih **int** object a um cia mi kha an hngaih/kawk veve. Cucaah `id(a)` le `id(b)` nih address aa khat an chuahnak a si.

Hihi **is** operator hmang in hneksak khawh a si. `a` le `b` nih object khat an hngaih caah **True** a chuah.

`a` chung ah value thar chiah kan i zuam tik ah, value aa dang (30) a si caah **int** object thar ser a si. Atu ah cun `a` nih **int** object thar kha a hngaih cang, asinain `b` nih cun **int** object value 3 kha a hngaih rih ko.

`a` nih value 3 a ngei mi **int** object a hngaih tiah chim nak in, `a` cu **int** object a si, asiloah 3 cu `a` ah assigned kan tuah tiah chim a si tawn.

Programmers tampi nih `a` le `b` cu **int** variables an si tiah an zumh, asinain atu ah cun a si lo ti kan hngalh cang.

### Problem 3.1

**Integer types** le **operators** hman ning hmuhsaknak.

<details>
<summary>Program</summary>

```python title="Problem 3.1"
# use of integer types (integer types hman ning)
print(3 / 4)
print(3 % 4)
print(3 // 4)
print(3 ** 4)

a = 10 ; b = 25 ; c = 15 ; d = 30 ; e = 2 ; f = 3 ; g = 5 
w = a + b - c 
x = d ** e 
y = f % g 
print(w, x, y)
h = 99999999999999999
i = 54321
print(h * i)
```
</details>

<details>
<summary>Output</summary>

```python title="Output"
0.75
3
0
81
20 900 3
5432099999999999945679
```
</details>

!!! note "Tips"
    * **3/4** nih 0 a chuah lo (Python 3 ah cun **0.75** a chuah, a tling lo mi nambar zong a tuak khawh).
    * Catlang khat chung ah **statements** tampi an um ahcun **;** (semicolon) hman in ṭhen ding a si.
    * **print(w, x, y)** nih **values** pawl kha **space** (karkhat) in ṭhen in a print/langhter.


### Problem 3.2

**float**, **complex** le **bool** types hman ning le cu hna he hman khawh mi **operators** hmuhsaknak.

<details>
<summary>Program</summary>

```python title="Problem 3.2"
# use of float (float hman ning)
i = 3.5
j = 1.2 
print(i % j) # 1.1 a chuah (approx)

# use of complex (complex number hman ning)
a = 1 + 2j 
b = 3 *(1 + 2j)
c = a * b
print(a)
print(b)
print(c)
print(a.real) # a i a real part (1.0)
print(a.imag) # a i a imaginary part (2.0)
print(a.conjugate( )) # a i a conjugate (1-2j)
print(a)

# use of bool (boolean hman ning)
x = True
y = 3 > 4 
print(x) # True
print(y) # False
```
</details>

<details>
<summary>Output</summary>

```python title="Output"
1.1
(1+2j)
(3+6j)
(-9+12j)
1.0
2.0
(1-2j)
(1+2j)
True
False
```
</details>

![Fig 3.1 Complex Number](../assests/complex%20number.jpg)

!!! note "Tips"
    * **%** (Modulus operator) hi **floats** cung zong ah a ṭuan kho.
    * **Complex number** pakhat in **real** le **imag** part kha lak khawh an si.
    * **Condition** (sining) pakhat chek a si tik ah **True** asiloah **False** in thlen a si.


### Problem 3.3

Number type pakhat in a dang ah thlen ning hmuhsaknak.

<details>
<summary>Program</summary>

```python title="Problem 3.3"
# convert to int (int ah thlen)
print(int(3.14)) # float in int ah (point hnu a hlonh)
a = int('485') # numeric string in int ah
b = int('768') # numeric string in int ah
c = a + b 
print(c)
print(int('1011', 2)) # binary in decimal int ah thlen
print(int('341', 8)) # octal in decimal int ah thlen
print(int('21', 16)) # hex in decimal int ah thlen

# convert to float (float ah thlen)
print(float(35)) # int in float ah
i = float('4.85') # numeric string in float ah
j = float('7.68') # numeric string in float ah
k = i + j 
print(k)

# convert to complex (complex ah thlen)
print(complex(35)) # int in complex ah
x = complex(4.85, 1.1) # numeric string in complex ah
y = complex(7.68, 2.1) # numeric string in complex ah
z = x + y 
print(z)

# convert to bool (bool ah thlen)
print(bool(35)) # True (0 a si lo mi paoh True an si)
print(bool(1.2)) # True
print(int(True)) # 1
print(int(False)) # 0
```
</details>

<details>
<summary>Output</summary>

```python title="Output"
3
1253
11
225
33
35.0
12.53
(35+0j)
(12.53+3.2j)
True
True
1
0
```
</details>


!!! note "Tips"
    * **Binary numeric string**, **octal numeric string** asiloah **hexadecimal numeric string** pawl kha a he aa khat mi **decimal integer** ah thlen khawh a si. Hi thil hi **float** caah tuah khawh a si lo.
    * **complex** ah thlen tik ah **argument** pakhat lawng hman a si ahcun, **imaginary part** cu `0` ah chiah a si.
    * **Zero** a si lo mi nambar (**int** asiloah **float**) paoh cu **True** tiah lak a si. `0` cu **False** tiah lak a si.

### Problem 3.4

**Built-in mathematical functions** (A chung um cia mi mathematical functions) hman ning hmuhsaknak program.

<details>
<summary>Program</summary>

```python title="Problem 3.4"
# built-in math functions (math functions hman ning)
print(abs(-25)) # 25 (Negative kha positive ah a thlen/Absolute value)
print(pow(2, 4)) # 16 (2 a voi 4 nak)
print(min(10, 20, 30, 40, 50)) # 10 (A hme bik)
print(max(10, 20, 30, 40, 50)) # 50 (A ngan bik)
print(divmod(17, 3)) # (5, 2) (Quotient 5 le Remainder 2 kha tuple in a chuah)
print(bin(64), oct(64), hex(64)) # Binary, Octal, Hexadecimal ah a thlen hna
print(round(2.567), round(2.5678, 2)) # 3 (A tling ah round a tuah), 2.57 (Point hnu 2 tiang round a tuah)

```
</details>

<details>
<summary>Output</summary>

```python title="Output"
25  
16
10
50
(5, 2)
0b1000000 0o100 0x40
3 2.57
```
</details>

!!! note "Tips"
    * **divmod(a, b)** nih a kop in **(a // b, a % b)** a chuah.
    * **bin( )**, **oct( )**, **hex( )** nih binary, octal le hexadecimal he aa khat mi values an chuah.
    * **round(x)** nih decimal point hnu ah 0 places (zeihmanh a um lo) tiang round tuah ding a si tiah a laak.

### Problem 3.5

**Math module** chung i functions hmang in program ṭial ning.

<details>
<summary>Program</summary>

```python title="Problem 3.5"
# mathematical functions from math module (math module chung i mathematical functions)
import math
x = 1.5357
print ( math.pi, math.e) # pi le e i an man pawl
print(math.sqrt( x)) # x i a square root
print(math.factorial(6)) # 6 i a factorial
print(math.fabs(x)) # x i a absolute value (float in)
print(math.log(x)) # x i a natural log
print(math.log10(x)) # x i a base-10 logarithm
print(math.exp(x)) # e a voi x nak (e raised to power x)
print(math.trunc(x)) # Integer ah thlen (point hnu hlonh)
print(math.floor(x)) # A niam deuh mi integer ah round (1)
print(math.ceil(x)) # A ngan deuh mi integer ah round (2)
print(math.trunc(-x)) # Integer ah thlen (-1)
print(math.floor(-x)) # A niam deuh mi integer ah round (-2)
print(math.ceil(-x)) # A ngan deuh mi integer ah round (-1)
print(math.modf(x)) # Fractional part le Integer part ṭhen in tuple in a chuah
```
</details>

<details>
<summary>Output</summary>

```python title="Output"
3.141592653589793 2.718281828459045
1.2392336341465238
720
1.5357
0.42898630314951025
0.1863063842699079
4.644575595215059
1
1
2
-1
-2
-1
(0.5357000000000001, 1.0)
```
</details>

!!! note "Tips"
    * **floor( )** nih **negative infinity** lei (a niam lei) ah a round, **ceil( )** nih **positive infinity** lei (a san lei) ah a round, **trunc( )** nih **0** lei ah a round (a niam lei asiloah a san lei siseh 0 umnak lei hoih in).
    * **Positive numbers** caah cun **trunc( )** cu **floor( )** he an i lo.
    * **Negative numbers** caah cun **trunc( )** cu **ceil( )** he an i lo.
    * **modf( )** nih nambar kop `(f, i)` a chuah, cu tik ah `x = f + i` a si i `0 <= f < 1` a si.

### Problem 3.6

**Float** le **integer** random numbers (nambar can-u-nan) sernak program ṭial tuah.

<details>
<summary>Program</summary>

```python title="Problem 3.6"
# random number operations using random module (random module hman ning)
import random 
import datetime

# datetime.time() hmang in seed tuah
# (Note: A ṭha deuh mi cu datetime.datetime.now() hman asiloah a lawng in chiah a si)
random.seed(datetime.time( )) 

print(random.random( )) # 0.0 le 1.0 karlak ah random float a chuah
print(random.random( )) # 0.0 le 1.0 karlak ah random float a chuah
print(random.randint(10, 100)) # 10 le 100 karlak ah random integer a chuah
```
</details>

!!! note "Tips" 
    * **seed( )** hi random number generator hram thoknak (initialize) caah hman a si.
    * **random.random( )** nih 0.0 in 1.0 karlak ah a um mi float value a chuah.
    * **random.randint(a, b)** nih a le b karlak ah a um mi integer value a chuah (a le b zong aa tel).

<details>
<summary>Output</summary>

```python title="Output"
0.23796462709189137
0.5442292252959519
57
```
</details>

!!! note "Tips"
    * **random** module kha **import** tuah a hau.
    * **Random number generation logic** kha atu lio caan (**current time**) he **seed** kan tuah ahcun, program kan **execute** (tuahter) fatin **random numbers** aa dang mi kan hmuh lai.
    * **random.seed( )** kha **parameter** tel lo in kan hman ahcun amah tein **current time** kha **seed** caah a hman.

### Problem 3.7

A tanglei hna hi **string**, **list**, **tuple**, **set** asiloah **dictionary** an si le si lo zeitin dah na hngalh/thleidan lai?

```text 
{10, 20, 30.5}
[1, 2, 3.14, 'Nagpur']
{12 : 'Simple', 43 : 'Complicated', 13 : 'Complex'}
"Check it out!"
3 + 2j
```

<details>
<summary>Program</summary>

```python title="Problem 3.7"
# determine type of data
print(type({10, 20, 30.5}))
print(type([1, 2, 3.14, 'Nagpur']))
print(type({12 : 'Simple', 43 : 'Complicated', 13 : 'Complex'}))
print(type("Check it out!"))
print(type(3 + 2j))
```
</details>

<details>
<summary>Output</summary>

```python title="Output"
<class 'set'>
<class 'list'>
<class 'dict'>
<class 'str'>
<class 'complex'>
```
</details>

!!! note "Tips"
    * **type( )** cu **built-in function** a si i, zeibantuk **data** (**built-in**, **container** asiloah **user-defined**) paoh i a **type** (a phun) kha a hngalh/thleidan khawh.


## **Exercises**

### **[A] A tanglei biahalnak hna hi phi tuah:**

* **a.** Variable `a` le `b` i an values (man) kha thlen (swap) nak program ṭial tuah. Variable pathumnak hman a ngah lo. `a` le `b` cung ah arithmetic (tuaknak) tuah a ngah lo.
* **b.** `math` module chung i a um mi **trigonometric functions** hman ning hmuhsaknak program ṭial tuah.
* **c.** 10 le 50 karlak ah random numbers (nambar can-u-nan) 5 sernak program ṭial tuah. **Seed value** ah 6 hmang tuah. Cun, program na execute (tuahter) fatin **seed value** aa thlen nakhnga time (caan) he pehtlai in tuah tuah?
* **d.** `trunc( )`, `floor( )` le `ceil( )` hna i an i dannak hngalh ding ah `-2.8`, `-0.5`, `0.2`, `1.5` le `2.9` pawl hmang in program ṭial tuah.
* **e.** City (Khuapi) pakhat i a lum-sik (temperature) kha Fahrenheit in chiah law (suum law), cucu Centigrade ah thlen nak program ṭial tuah. An pahnih in print (langhter) tuah.
* **f.** Triangle (Tukum) pakhat i a sir (sides) `a`, `b`, `c` ngeih a si. A kil (angles) pathum tuak nak program ṭial tuah, a phi cu a niam bik integer (next integer) ah round tuah. A tanglei formulae hi hmang:

$$ a^2 = b^2 + c^2 - 2bc.cos A, b^2 = a^2 + c^2 - 2ac.cos B, c^2 = a^2 + b^2 - 2ab.cos C$$


### **[B] A tanglei rian pawl hi zeitin dah na tuah hna lai:**

* **a.** `2 + 3j` i a **imaginary part** kha **print** tuah.
* **b.** `4 + 2j` i a **conjugate** kha la/chuah.
* **c.** **Binary** `1100001110` he aa khat mi **decimal** kha **print** tuah.
* **d.** **Float value** `4.33` kha **numeric string** ah thlen.
* **e.** `29` kha `5` in cheu tik i a chuak mi **integer quotient** (a cheu tu) le **remainder** (a taang mi) kha lak ding.
* **f.** **Decimal** `34567` he aa khat mi **hexadecimal** kha lak ding.
* **g.** `45.6782` kha **decimal place** pahnihnak tiang **round-off** tuah.
* **h.** `3.556` chung in `4` lak ding.
* **i.** `16.7844` chung in `17` lak ding.
* **j.** `3.45` kha `1.22` in cheu tik i a **remainder** (a taang mi) lak ding.

### **[C] A tanglei pawl lak ah a khoi mi hi dah variable min caah hman a ngah lo (invalid), cun zeiruang ah dah?**

| Column 1 | Column 2 | Column 3 | Column 4 |
|---|---|---|---|
| BASICSALARY | _basic | basic-hra | #MEAN |
| group. | 422 | pop in 2020 | over |
| timemindovermatter | SINGLE | hELLO | queue. |
| team'svictory | Plot#3 | 2015_DDay | |

### **[D] A tanglei expressions pawl hi tuak hna:**

* **a.** `2 ** 6 // 8 % 2`
* **b.** `9 ** 2 // 5 - 3`
* **c.** `10 + 6 - 2 % 3 + 7 - 2`
* **d.** `5 % 10 + 10 - 23 * 4 // 3`
* **e.** `5 + 5 // 5 - 5 * 5 ** 5 % 5`
* **f.** `7 % 7 + 7 // 7 - 7 * 7`

### **[E] A tanglei expressions pawl hi tuak hna:**

* **a.** `min(2, 6, 8, 5)`
* **b.** `bin(46)`
* **c.** `round(10.544336, 2)`
* **d.** `math.hypot(6, 8)`
* **e.** `math.modf(3.1415)`

### **[F] A tanglei pawl hi a kop in thleidan/peh hna:**

| Section A | Section B |
|---|---|
| **a.** complex | 1. `\` |
| **b.** Escape special character (Special character hrialnak) | 2. Container type |
| **c.** Tuple | 3. Basic type |
| **d.** Natural logarithm | 4. `log( )` |
| **e.** Common logarithm | 5. `log10( )` |



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
