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

### 3.1 Identifiers and Keywords

Python က **Case sensitive language** တစ်ခုပါ။ **Python identifier** ဆိုတာက **Variable**၊ **Function**၊ **Class**၊ **Module** သို့မဟုတ် တခြား **Object** တွေကို ခွဲခြားသိနိုင်ဖို့ ပေးထားတဲ့ နာမည်တစ်ခု ဖြစ်ပါတယ်။ **Identifiers** တွေ ဖန်တီးတဲ့အခါ လိုက်နာရမယ့် စည်းကမ်းတွေကတော့ -

- **Alphabet** (အက္ခရာ) သို့မဟုတ် **Underscore** (_) နဲ့ စရပါမယ်။

- အဲဒီနောက်မှာ စာလုံးတွေ၊ _ ၊ နဲ့ **Digits** (ဂဏန်း) တွေ လိုက်လို့ရပါတယ်။

- **Keyword** တွေကို **Identifier** အနေနဲ့ သုံးလို့ မရပါဘူး။

**Keywords** အားလုံးက **Lowercase** (အက္ခရာအသေး) တွေ ဖြစ်ပါတယ်။ Python မှာ **Keywords** စုစုပေါင်း (၃၃) လုံးရှိပြီး *Table 3.1* မှာ ဖော်ပြထားပါတယ်။

|Table 3.1 Keywords list|-/-|-/-|-/-|
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

**Python keywords** စာရင်းကို အောက်ပါ **Statements** တွေသုံးပြီး ထုတ်ကြည့်လို့ ရပါတယ် -

```python title="checking keyword list"
import keyword # 'keyword' module ကို သုံးလို့ရအောင် ခေါ်လိုက်တာ
print(keyword.kwlist) # syntax ကတော့ modulename.object/function ပုံစံပါ
```

---

### 3.2 Python Types

**Python** မှာ **Data types** (၃) မျိုး (၃) စား ရှိပါတယ် -

- **Basic Types**:
    * **int**, **float**, **complex**, **bool**, **string**, **bytes**
- **Container Types**:
    * **list**, **tuple**, **set**, **dict**
- **User-defined types**:
    * **class**

ဒီအထဲမှာ **Basic types** အကြောင်းကို ဒီ Chapter မှာ အသေးစိတ် ရှင်းပြသွားပါမယ်။ **Container types** အကြောင်းကိုတော့ အကြမ်းဖျင်းပဲ ပြောသွားပါမယ်။ **Container type** တစ်ခုစီအတွက် သီးသန့် Chapter တွေနဲ့ အသေးစိတ် ထပ်ရှင်းပြပေးထားပါတယ်။ **User-defined types** အကြောင်းကိုတော့ ဒီ Chapter မှာ မပြောတော့ပါဘူး။ **Chapter 17** ကျမှ ဘယ်လိုဖန်တီးမလဲ၊ ဘယ်လိုသုံးမလဲဆိုတာ ဆွေးနွေးသွားပါမယ်။

---

#### 3.2.1 Basic Types

**Basic types** အမျိုးမျိုးရဲ့ ဥပမာတွေကို အောက်မှာ ဖော်ပြပေးထားပါတယ် -

* **int** ကို **binary**, **decimal**, **octal**, **hexadecimal** ပုံစံတွေနဲ့ ဖော်ပြလို့ရပါတယ်။
* **binary** ဆိုရင် 0b/0B ၊ **octal** ဆိုရင် 0o/0O ၊ **hex** ဆိုရင် 0x/0X နဲ့ စပါတယ်။ (ဥပမာ - 0b10111, 156, 0o432, 0x4A3)
* **float** ကို **fractional** (ဒသမကိန်း) သို့မဟုတ် **exponential form** (ထပ်ကိန်းပုံစံ) နဲ့ ဖော်ပြလို့ရပါတယ်။ (ဥပမာ - 314.1528, 3.141528e2, 3.141528E2)
* **complex** မှာ **real** နဲ့ **imaginary part** ဆိုပြီး ပါပါတယ်။ (ဥပမာ - 3 + 2j, 1 + 4J)
* **bool** က **Boolean values** နှစ်ခုထဲက ကြိုက်တာတစ်ခု ဖြစ်နိုင်ပြီး နှစ်ခုလုံးက အက္ခရာအကြီးနဲ့ စပါတယ်။ (ဥပမာ - **True**, **False**)
* **string** ဆိုတာ `' '`, `" "`, သို့မဟုတ် `""" """` တွေကြားထဲမှာ ရေးထားတဲ့ **Immutable collection of Unicode characters** ဖြစ်ပါတယ်။ ဥပမာ - 'Rosanna', "Rosanna", """Rosanna"""။
* **bytes** က **Binary data** ကို ကိုယ်စားပြုပါတယ်။

```python title="bytes example"
b'\xa1\xe4\x56' # hex values a1a456 ပါတဲ့ 3 bytes ကို ကိုယ်စားပြုပါတယ်
```
Data တစ်ခုချင်းစီရဲ့ **Type** ကို **type( )** လို့ခေါ်တဲ့ **Function** သုံးပြီး အောက်ပါအတိုင်း စစ်ဆေးနိုင်ပါတယ် -

```python title="checking type of data using type() function"
print(type(35)) # <class 'int'> ဆိုပြီး print ထုတ်ပေးပါလိမ့်မယ်
print(type(3.14)) # <class 'float'> ဆိုပြီး print ထုတ်ပေးပါလိမ့်မယ်
```
#### 3.2.2 Integer and Float Ranges

* **int** တွေက **Arbitrary size** ဖြစ်တဲ့အတွက် ကြိုက်သလောက် အရွယ်အစား ထားလို့ရပါတယ်။ (Memory ဆန့်သရွေ့ ဂဏန်းအလုံးရေ အကန့်အသတ်မရှိပါဘူး)။

```python title="integer example"
a = 123
b = 1234567890
c = 123456789012345678901234567890
```
Python မှာ **Arbitrary precision integers** ရှိပါတယ်။ ဒါကြောင့် ကိုယ်လိုချင်သလောက် ဂဏန်းအကြီးကြီးတွေ ဖန်တီးလို့ရတယ်။ နောက်ပြီး **Overflow** သို့မဟုတ် **Underflow** ဖြစ်မှာ ပူစရာမလိုဘဲ **Integers** တွေကို **Arithmetic operations** လုပ်ဆောင်နိုင်ပါတယ်။

**Floats** တွေကိုတော့ **Internal** မှာ **IEEE 754 standard** အရ **Binary** ပုံစံနဲ့ **64-bit double-precision values** အနေနဲ့ သိမ်းဆည်းပါတယ်။ ဒီ **Standard** အရ **Float** တစ်ခုရဲ့ အကြီးဆုံးတန်ဖိုး (Maximum value) က ခန့်မှန်းခြေ **1.8 x 10^308** ဖြစ်ပါတယ်။ ဒီထက်ကြီးတဲ့ ကိန်းဂဏန်းဆိုရင် **inf** (**infinity** အတိုကောက်) အနေနဲ့ ဖော်ပြပါလိမ့်မယ်။ 

**Floats** တော်တော်များများကို **Binary form** နဲ့ 'တိတိကျကျ' (Exactly) ဖော်ပြလို့ မရနိုင်ပါဘူး။ ဒါကြောင့် **Internal representation** က တကယ့်တန်ဖိုးရဲ့ **Approximation** (နီးစပ်ဆုံးတန်ဖိုး) သာ ဖြစ်လေ့ရှိပါတယ်။

တကယ့်တန်ဖိုးနဲ့ **Represented value** ကြားက ကွာဟချက်က အရမ်းသေးငယ်တဲ့အတွက် ပုံမှန်အားဖြင့်တော့ ပြဿနာကြီးကြီးမားမား မဖြစ်စေပါဘူး။

### 3.3 Variable Type and Assignment

**Variable** တစ်ခုရဲ့ **Type** ကို ကြိုပြီး သတ်မှတ်ပေးစရာ (Define) မလိုပါဘူး။ **Execution** လုပ်နေတဲ့အချိန်ကျမှ သူအသုံးပြုနေတဲ့ **Context** ပေါ်မူတည်ပြီး **Variable type** ကို အလိုအလျောက် ဆုံးဖြတ် (**Infer**) သွားတာပါ။ ဒါကြောင့် Python ကို **Dynamically-typed language** လို့ ခေါ်တာဖြစ်ပါတယ်။

```python title="Variable type"
a = 25 # a ရဲ့ type ကို int လို့ ယူဆလိုက်ပါတယ်
a = 31.4 # a ရဲ့ type ကို float လို့ ယူဆလိုက်ပါတယ်
a = 'Hi' # a ရဲ့ type ကို str လို့ ယူဆလိုက်ပါတယ်
```

**Variable** တစ်ခုရဲ့ **Type** ကို **Built-in function** ဖြစ်တဲ့ **type()** ကို သုံးပြီး စစ်ဆေးနိုင်ပါတယ်။

```python title="str variable"
a = 'Job Kaa'
print(type(a)) # type ကို str အနေနဲ့ ဖော်ပြပေးပါလိမ့်မယ်
```

Simple variable assignment:

```python title="assignment example"
a = 10 
pi = 3.14 
name = 'Rosanna'
```

**Variables** အများကြီးကို တစ်ပြိုင်နက် **Assignment** လုပ်ခြင်း -

```python title="multiple assignment example"
a = 10 ; pi = 31.4 ; name = 'Rosanna' # ; ကို statement separator အနေနဲ့ သုံးထားတာပါ
a, pi, name = 10, 3.14, 'Rosanna'
a = b = c = d = 5
```

#### 3.3.1 Arithmetic Operators

**Arithmetic Operators**: **`+, - , * , /, %, //, **`**

```python title="Arithmetic Operators"
a = 4 / 2 # True division လုပ်ဆောင်ပြီး Float 2.0 ကို ရရှိပါတယ်
a = 7 % 2 # % က အကြွင်း (Remainder) 1 ကို ပေးပါတယ်
b = 3 ** 4 # ** က ထပ်ကိန်းတင်ပေးပါတယ် (3 raised to 4)
c = 4 // 3 # // က ဒသမပိုင်းတွေကို ဖယ်ထုတ်ပြီး စားလဒ် (Quotient) 1 ကိုပဲ ယူပါတယ်
```

**In-place assignment operators** တွေက **Arithmetic operations** တွေလုပ်ဖို့အတွက် **Shortcut** ကောင်းကောင်းတစ်ခု ဖြစ်ပါတယ်။ သူတို့ထဲမှာ **`+=, -=, *=, /=, %=, //=, **=`** တို့ ပါဝင်ပါတယ်။

```python title="In-place assignment"
a **= 3 # a = a ** 3 နဲ့ အတူတူပါပဲ
b %= 10 # b = b % 10 နဲ့ အတူတူပါပဲ
```

### 3.3.2 Operation Nuances

**Floor division** (`a//b`) လုပ်ဆောင်တဲ့အခါ ရလာမယ့် **Result** က **Quotient** (စားလဒ်) ထက် ငယ်တဲ့ (သို့မဟုတ်) ညီတဲ့အထဲက အကြီးဆုံး **Integer** ဖြစ်ပါတယ်။ `//` ကို **Floor division operator** လို့ ခေါ်ပါတယ်။



ရိုးရိုးလေး မှတ်မယ်ဆိုရင်တော့ **Number line** ပေါ်မှာ ဘယ်ဘက် (တန်ဖိုးပိုငယ်တဲ့ဘက်) ကို အမြဲတမ်း 'Floor' (အောက်ချ) လိုက်တယ်လို့ မှတ်ယူနိုင်ပါတယ်။ ဒါကြောင့် -3.33 ဆိုရင် -3 မဖြစ်ဘဲ -4 ဖြစ်သွားတာပါ။

```python title="Floor Division"
print(10 // 3) # 3 ကို ရပါတယ် (3.33... ထက် ငယ်တဲ့/ညီတဲ့ integer)
print(-10 // 3) # -4 ကို ရပါတယ် (-3.33... ထက် ငယ်တဲ့ integer က -4 ပါ)
print(10 // -3) # -4 ကို ရပါတယ်
print(-10 // -3) # 3 ကို ရပါတယ်
print(3 // 10) # 0 ကို ရပါတယ် (0.3 ထက် ငယ်တဲ့/ညီတဲ့ integer)
print(3 // -10) # -1 ကို ရပါတယ် (-0.3 ထက် ငယ်တဲ့ integer က -1 ပါ)
print(-3 // 10) # -1 ကို ရပါတယ်
print(-3 // -10) # 0 ကို ရပါတယ်
```

**-10 // 3** မှာ -10 ရဖို့ 3 နဲ့စားလိုက်ရင် -3.333 ရပါတယ်၊ သူ့ရဲ့ **Floor value** (အောက်ချလိုက်တဲ့ တန်ဖိုး) က -4 ဖြစ်ပါတယ်။

**10 // -3** မှာ 10 ရဖို့ -3 နဲ့စားလိုက်ရင် -3.333 ရပါတယ်၊ သူ့ရဲ့ **Floor value** က -4 ဖြစ်ပါတယ်။

**-10 // -3** မှာ -10 ရဖို့ -3 နဲ့စားလိုက်ရင် 3.333 ရပါတယ်၊ သူ့ရဲ့ **Floor value** က 3 ဖြစ်ပါတယ်။

**print( )** ဆိုတာ **Screen** ပေါ်မှာ **Output** ထုတ်ပေးဖို့ သုံးတဲ့ **Function** တစ်ခုပါ။ သူ့ကို ပုံစံမျိုးစုံနဲ့ သုံးလို့ရပါတယ်။ **Chapter 7** ရောက်ရင် အသေးစိတ် ဆွေးနွေးပါမယ်။

**a % b** **Operation** ကို **a - (b * (a // b))** ဆိုတဲ့ ပုံသေနည်းအတိုင်း **Evaluate** လုပ် (တွက်ချက်) ပါတယ်။ 

ဒါကို အောက်က ဥပမာတွေကြည့်ရင် အရှင်းဆုံး နားလည်ပါလိမ့်မယ် -

```python title="print functions"
print(10 % 3) # 1 ရပါတယ် (ပုံမှန် အကြွင်းပါ)
print(-10 % 3) # 2 ရပါတယ် (Formula: -10 - (3 * -4) = -10 + 12 = 2)
print(10 % -3) # -2 ရပါတယ် (Formula: 10 - (-3 * -4) = 10 - 12 = -2)
print(-10 % -3) # -1 ရပါတယ် (Formula: -10 - (-3 * 3) = -10 + 9 = -1)
print(3 % 10) # 3 ရပါတယ်
print(3 % -10) # -7 ရပါတယ် (Formula: 3 - (-10 * -1) = 3 - 10 = -7)
print(-3 % 10) # 7 ရပါတယ် (Formula: -3 - (10 * -1) = -3 + 10 = 7)
print(-3 % -10) # -3 ရပါတယ်
```

**`a % b`** ကို `a - (b * (a // b))` ဆိုပြီး **Evaluate** လုပ်တဲ့အတွက်ကြောင့်၊
**`-10 % 3`** ဆိုရင် `-10 - (3 * (-10 // 3))` လို့ တွက်ပါတယ်၊ ဒါကြောင့် ရလဒ် **2** ကို ရပါတယ်။
**`10 % -3`** ဆိုရင် `10 - (-3 * (10 // -3))` လို့ တွက်ပါတယ်၊ ဒါကြောင့် รလဒ် **-2** ကို ရပါတယ်။
**`-10 % -3`** ဆိုရင် `-10 - (-3 * (-10 // -3))` လို့ တွက်ပါတယ်၊ ဒါကြောင့် ရလဒ် **-1** ကို ရပါတယ်။

**Mathematical rule** အရ *`a / b x c`* နဲ့ *`a x c / b`* က တူတယ်ဆိုပေမယ့်၊ **Programming** မှာ အမြဲတမ်းတော့ မမှန်ပါဘူး။ (အထူးသဖြင့် ဂဏန်းအကြီးကြီးတွေ တွက်တဲ့အခါမျိုးမှာပေါ့)။

```python title="Mathematical rule"
# အောက်ပါ expressions တွေက results အတူတူပဲ ထွက်ပါတယ်
a = 300 / 100 * 250
a = 300 * 250 / 100

# ဒါပေမယ့် ဒီဟာတွေကတော့ မတူတော့ပါဘူး
b = 1e210 / 1e200 * 1e250
b = 1e210 * 1e250 / 1e200 # INF (Infinity) ထွက်သွားပါတယ်
```

**True** ဆိုတာ `1`၊ **False** ဆိုတာ `0` ဖြစ်တဲ့အတွက် သူတို့ကို ဂဏန်းတွေလိုပဲ ပေါင်းလို့ရပါတယ်။

```python title="True and False"
a = True + True # 2 ရပါတယ် (1 + 1)
b = True + False # 1 ရပါတယ် (1 + 0)
```

### 3.4 Precedence and Associativity

**Arithmetic expression** တစ်ခုမှာ **Operators** တွေ အများကြီး ပါလာတဲ့အခါ၊ အဲဒီ **Operators** တွေရဲ့ **Precedence** (ဦးစားပေးအဆင့်/Priority) ပေါ်မူတည်ပြီး **Evaluate** လုပ် (တွက်ချက်) ပါတယ်။ 

**Priority** အမြင့်ဆုံးကနေ အနိမ့်ဆုံးအလိုက် စီထားတဲ့ **Operators** တွေကတော့ **(PEMDAS)** အတိုင်း ဖြစ်ပါတယ် -

```python title="Precedence of operators"
( )          # Parentheses (ကွင်းများ)
** # Exponentiation (ထပ်ကိန်းတင်ခြင်း)
*, /, //, %  # Multiplication, Division (အမြှောက်၊ အစား အုပ်စု)
+, -         # Addition, Subtraction (အပေါင်း၊ အနုတ် အုပ်စု)
```
**Precedence** (Priority) တူနေတဲ့ **Operators** တွေ ပါလာခဲ့ရင်တော့ **Associativity** ကို ကြည့်ပြီး ဘယ်ကောင် အရင်လုပ်မလဲဆိုတာ ဆုံးဖြတ်ပါတယ်။

**Operator** တိုင်းမှာ **Left to right associativity** (ဘယ်မှ ညာသို့) သို့မဟုတ် **Right to left associativity** (ညာမှ ဘယ်သို့) ဆိုတာ ရှိကြပါတယ်။

ဥပမာ - `c = a * b / c` ဆိုတဲ့ **Expression** မှာ `*` နဲ့ `/` က **Priority** တူပါတယ်။ ဒါပေမယ့် **Arithmetic operators** တွေက **Left to right associativity** ရှိတဲ့အတွက် `*` ကို `/` ထက် အရင်လုပ်ပါတယ်။ (ဘယ်ဘက်အခြမ်းက ကောင်ကို အရင်လုပ်တာပါ)။

**Python operators** အားလုံးရဲ့ **Priority** နဲ့ **Associativity** စာရင်းအပြည့်အစုံကို **Appendix A** မှာ ကြည့်ရှုနိုင်ပါတယ်။

#### 3.4.1 Conversions

**Mixed mode operations** (Type မတူတာတွေ ရောပြီး တွက်ခြင်း): 

- **int** နဲ့ **float** တွဲလုပ်ရင် **float** ရပါမယ်။
- **int** နဲ့ **complex** တွဲလုပ်ရင် **complex** ရပါမယ်။
- **float** နဲ့ **complex** တွဲလုပ်ရင် **complex** ရပါမယ်။

**Built-in functions** တွေဖြစ်တဲ့ **int( )**, **float( )**, **complex( )** နဲ့ **bool( )** တို့ကို သုံးပြီး **Numeric type** တစ်ခုကနေ နောက်တစ်ခုကို ပြောင်းလဲ (**Convert**) နိုင်ပါတယ်။

**Type conversions:**

```python title="Type conversions"
int(float/numeric string) # float သို့မဟုတ် numeric string ကို int ပြောင်းခြင်း
int(numeric string, base) # numeric string ကို base တစ်ခုခုအလိုက် int ပြောင်းခြင်း
float(int/numeric string) # int သို့မဟုတ် numeric string ကို float ပြောင်းခြင်း
float(int) # int ကို float ပြောင်းခြင်း
complex(int/float) # complex ပြောင်းခြင်း (imaginary part က 0 ဖြစ်နေမယ်)
complex(int/float, int/float) # complex ပြောင်းခြင်း (real, imag နှစ်ခုလုံးပါမယ်)
bool(int/float) # int/float ကို True/False (1/0) ပြောင်းခြင်း
str(int/float/bool) # string အဖြစ် ပြောင်းခြင်း
chr(int) # int တန်ဖိုးနဲ့ သက်ဆိုင်တဲ့ character (ASCII/Unicode) ကို ထုတ်ပေးခြင်း
```

**int( )** က **Decimal portion** (ဒသမပိုင်း) ကို ဖြတ်ထုတ်လိုက်တာဖြစ်တဲ့အတွက် အမြဲတမ်း **Zero** ဘက်ကိုပဲ **Round** လုပ်သွားပါတယ် (**Rounds towards zero** ဖြစ်ပါတယ်)။ 

```python title="int()"
a = int(3.33) # 3 ရပါတယ်
b = int(-3.33) # -3 ရပါတယ်
```

#### 3.4.2 Built-in Functions

Python မှာ **Program** ရဲ့ ဘယ်နေရာမှာမဆို အချိန်မရွေး ခေါ်သုံးလို့ရတဲ့ **Built-in functions** တွေ အများကြီး ပါပါတယ်။ ကျွန်တော်တို့ **Output** ကို **Screen** ပေါ်ထုတ်ဖို့ သုံးနေကျ **print( )** function ကလည်း **Built-in function** တစ်ခုပါပဲ။

**Built-in function** တစ်ခုခုအကြောင်း **Help** လိုချင်ရင် **help(function)** ကို သုံးပြီး ကြည့်လို့ရပါတယ်။

**Numbers** တွေနဲ့ တွဲသုံးလေ့ရှိတဲ့ **Built-in functions** တွေကို အောက်မှာ ဖော်ပြထားပါတယ် -

```python title="Built-in functions"
abs(x) # x ရဲ့ Absolute value (ပကတိတန်ဖိုး) ကို ပြန်ပေးပါတယ်
pow(x, y) # x ရဲ့ y ထပ်ကိန်းတန်ဖိုး (x raised to y) ကို ပြန်ပေးပါတယ်
min(x1, x2,...) # ပေးထားတဲ့ထဲက အငယ်ဆုံးတန်ဖိုး (Smallest argument) ကို ပြန်ပေးပါတယ်
max(x1, x2,...) # ပေးထားတဲ့ထဲက အကြီးဆုံးတန်ဖိုး (Largest argument) ကို ပြန်ပေးပါတယ်
divmod(x, y) # (x // y, x % y) ဆိုပြီး စားလဒ်နဲ့ အကြွင်းအတွဲ (Pair) ကို ပြန်ပေးပါတယ် 
round(x [,n]) # x ကို ဒသမနေရာ n ခုအထိ ဖြတ်ပြီး (Round လုပ်ပြီး) ပြန်ပေးပါတယ် 
bin(x) # x ရဲ့ Binary equivalent (Binary တန်ဖိုး) ကို ပြန်ပေးပါတယ်
oct(x) # x ရဲ့ Octal equivalent (Octal တန်ဖိုး) ကို ပြန်ပေးပါတယ်
hex(x) # x ရဲ့ Hexadecimal equivalent (Hexadecimal တန်ဖိုး) ကို ပြန်ပေးပါတယ်
```

အောက်ပါ **Python program** မှာ ဒီ **Built-in functions** တွေထဲက တချို့ကို ဘယ်လိုသုံးရမလဲဆိုတာ ပြထားပါတယ် -

```python title="Built-in functions"
a = abs(-3) # a ထဲကို 3 ထည့်လိုက်ပါတယ်
print(min(10, 20, 30, 40)) # 10 ကို print ထုတ်ပေးပါတယ်
print(hex(26)) # 1a (hex value) ကို print ထုတ်ပေးပါတယ်
```

#### 3.4.3 Built-in Modules

**Built-in functions** တွေအပြင်၊ Python မှာ **Built-in modules** တွေလည်း အများကြီး ပါဝင်ပါတယ်။ **Module** တစ်ခုစီမှာ **Functions** တွေ အများကြီး ပါဝင်ပါတယ်။
အဆင့်မြင့် **Mathematical operations** တွေ လုပ်ဆောင်ဖို့အတွက် **Built-in modules** တွေဖြစ်တဲ့ **math**, **cmath**, **random**, **decimal** တို့ထဲက **Functions** တွေကို အသုံးပြုနိုင်ပါတယ်။

```python title="Built-in modules"
math - အသုံးဝင်တဲ့ mathematics functions တွေ အများကြီး ပါပါတယ်။
cmath - complex numbers တွေပေါ်မှာ operations လုပ်ဖို့ functions တွေ ပါပါတယ်။
random - random number generation (ဂဏန်းတွေ ကျပန်းထုတ်ပေးတာ) နဲ့ ပတ်သက်တဲ့ functions တွေ ပါပါတယ်။
decimal - တိကျသေချာတဲ့ arithmetic operations တွေ လုပ်ဖို့ functions တွေ ပါပါတယ်။
```

**math** module ထဲက **Mathematical functions** များ:

```python title="Mathematical functions in math module"
pi, e # pi နဲ့ e constants တွေရဲ့ တန်ဖိုးများ
sqrt(x) # x ရဲ့ Square root
factorial(x) # x ရဲ့ Factorial
fabs(x) # Float x ရဲ့ Absolute value
log(x) # x ရဲ့ Natural log (log to the base e)
log10(x) # x ရဲ့ Base-10 logarithm
exp(x) # e ရဲ့ x ထပ်ကိန်း (e raised to x)
trunc(x) # Integer ဖြစ်အောင် ဖြတ်ထုတ်လိုက်ခြင်း (Truncate)
ceil(x) # x နဲ့ ညီတဲ့ (သို့) x ထက်ကြီးတဲ့အထဲက အငယ်ဆုံး Integer (Ceiling) 
floor(x) # x နဲ့ ညီတဲ့ (သို့) x ထက်ငယ်တဲ့အထဲက အကြီးဆုံး Integer (Floor)
modf(x) # x ရဲ့ Fractional နဲ့ Integer parts တွေကို ခွဲထုတ်ပေးခြင်း
```

**round( )** **built-in function** က **Decimal places** (ဒသမနေရာ) အရေအတွက် သတ်မှတ်ပြီး **Round** လုပ်လို့ရပေမယ့်၊ **math module** ရဲ့ **Library functions** တွေဖြစ်တဲ့ **trunc( )**၊ **ceil( )** နဲ့ **floor( )** တွေကတော့ အမြဲတမ်း **Decimal places** မပါအောင် (Zero decimal places အထိ) **Round** လုပ်ပေးပါတယ်။

**math module** ထဲက **Trigonometric functions** များ: 

```python title="Trigonometric functions in math module"
degrees(x) # Radians ကနေ Degrees သို့ ပြောင်းခြင်း
radians(x) # Degrees ကနေ Radians သို့ ပြောင်းခြင်း
sin(x) # x Radians ရဲ့ Sine တန်ဖိုး
cos(x) # x Radians ရဲ့ Cosine တန်ဖိုး
tan(x) # x Radians ရဲ့ Tan တန်ဖိုး
sinh(x) # x ရဲ့ Hyperbolic sine
cosh(x) # x ရဲ့ Hyperbolic cosine
tanh(x) # x ရဲ့ Hyperbolic tan
acos(x) # x ရဲ့ Cos inverse (Radians နဲ့ ရပါမယ်)
asin(x) # x ရဲ့ Sine inverse (Radians နဲ့ ရပါမယ်)
atan(x) # x ရဲ့ Tan inverse (Radians နဲ့ ရပါမယ်)
hypot(x, y) # sqrt(x * x + y * y) (ထောင့်မှန်ခံအနား ရှာခြင်း)
```

**random module** ကနေ **Random number generation** လုပ်ပေးတဲ့ **Functions** များ:

```python title="Random number generation functions from random module"
random( ) # 0 နဲ့ 1 ကြားက random number တစ်ခု ထုတ်ပေးပါတယ်
randint(start, stop) # သတ်မှတ်ထားတဲ့ range ထဲက random number တစ်ခု ထုတ်ပေးပါတယ်
seed( ) # random number generation logic အတွက် current time ကို seed အနေနဲ့ သတ်မှတ်ပါတယ်
seed(x) # random number generation logic အတွက် x ကို seed အနေနဲ့ သတ်မှတ်ပါတယ်
```
**Module** တစ်ခုထဲမှာရှိတဲ့ **Functions** တွေကို အသုံးပြုဖို့အတွက် **import statement** ကိုသုံးပြီး အဲဒီ **Module** ကို **import** လုပ်ပေးဖို့ လိုအပ်ပါတယ်။

အောက်ပါ **Python program** မှာ **math module** နဲ့ **random module** ထဲက **Functions** တချို့ကို ဘယ်လိုအသုံးပြုလဲဆိုတာ ပြသထားပါတယ် -

```python title="Using functions from math and random modules"
import math
import random
print(math.factorial(5)) # 120 ကို print ထုတ်ပေးပါတယ်
print(math.degrees(math.pi)) # 180.0 ကို print ထုတ်ပေးပါတယ်
print(random.random( )) # 0.8960522546341796 (ကျပန်းဂဏန်းတစ်ခု) ကို print ထုတ်ပေးပါတယ်
```
**Built-in functions** တွေရော၊ **Built-in module** တစ်ခုချင်းစီမှာပါတဲ့ **Functions** တွေရောက အများကြီးဗျ။ ဒီ **Functions** နာမည်တွေကို အကုန်လိုက်မှတ်မိနေဖို့ဆိုတာ မလွယ်ပါဘူး (မေ့တတ်ကြပါတယ်)။ အောက်က **Program** လေးကို run ပြီး ဘာတွေပါလဲဆိုတာ အမြန် **List** ထုတ်ကြည့်လို့ရပါတယ် -

```python title="Getting list of built-in functions"
import math
print(dir(__builtins__)) # builtins ရဲ့ ရှေ့နဲ့နောက်မှာ underscores 2 ခုစီ ပါပါတယ်
print(dir(math))
```
### 3.5 Container Types

**Container types** ဆိုတာက ပုံမှန်အားဖြင့် **Values** အများကြီးကို တစုတစည်းတည်း သိမ်းဆည်းထားတာကို ဆိုလိုပါတယ်။ **Container types** အမျိုးမျိုးရဲ့ ဥပမာတွေကို အောက်မှာ ဖော်ပြထားပါတယ် -


```python title="Container types"
# list ဆိုတာက တူတာတွေရော၊ မတူတာတွေရော ရောနှောသိမ်းဆည်းလို့ရတဲ့ indexed collection တစ်ခုပါ
[10, 20, 30, 20, 30, 40, 50, 10], ['She', 'sold', 10, 'shells']

# tuple ဆိုတာက ပြင်ဆင်လို့မရတဲ့ immutable collection တစ်ခုပါ
('Rosanna', 34, 4500.55), ('Let Us Python', 350, 195.00)

# set ဆိုတာက unique values (ထပ်နေတာ မပါတဲ့ တန်ဖိုး) တွေကို စုစည်းထားတာပါ
{10, 20, 30, 40}, {'Rosanna', 34, 45000}

# dict ဆိုတာက key-value pairs တွေကို စုစည်းထားတာဖြစ်ပြီး၊ unique key တွေကို '' ကြားထဲမှာ ထားရပါတယ်
{'ME101' : 'Strength of materials', 'EE101' : 'Electronics'}
```
**List** နဲ့ **Tuple** ထဲက **Values** တွေကို သူတို့ရဲ့ **Position** (နေရာ) သတ်မှတ်ချက်ကို သုံးပြီး **Access** လုပ်လို့ရပါတယ်။ **Set** ထဲက **Values** တွေကိုတော့ **for loop** သုံးပြီး **Access** လုပ်နိုင်ပါတယ် (**Chapter 6** မှာ ဆွေးနွေးပါမယ်)။ **Dictionary** ထဲက **Values** တွေကိုတော့ **Key** ကို အသုံးပြုပြီး **Access** လုပ်နိုင်ပါတယ်။

အောက်ပါ **Program** မှာ ဒါတွေကို ဘယ်လိုလုပ်လဲဆိုတာ ပြထားပါတယ် -

```python title="Accessing values in container types"
lst = [10, 20, 30, 20, 30, 40, 50, 10]
tpl = ('Let Us Python', 350, 195.00)
s = {10, 20, 30, 40}
dct = {'ME101' : 'SOM', 'EE101' : 'Electronics'}

# List နဲ့ Tuple ကို Index (Position) သုံးပြီး Access လုပ်ခြင်း
print(lst[0], tpl[2]) # 10 နဲ့ 195.0 ကို print ထုတ်ပေးပါတယ်

# Dictionary ကို Key သုံးပြီး Access လုပ်ခြင်း
print(dct['ME101']) # SOM ကို print ထုတ်ပေးပါတယ်
```

#### 3.5.1 Python Type Jargon

Python **Types** တွေအကြောင်း ပြောတဲ့အခါ အောက်ပါ **Terms** (ဝေါဟာရ) တွေကို မကြာခဏ သုံးလေ့ရှိပါတယ် -

* **Collection** - **Container types** တွေကို ယေဘုယျခေါ်တဲ့ အခေါ်အဝေါ်ပါ။

* **Iterable** - **Loop** ပတ်ပြီး အထဲက တန်ဖိုးတွေကို တစ်ခုချင်းစီ ဆွဲထုတ်အသုံးပြုလို့ရတဲ့ **Collection** မျိုးကို ဆိုလိုတာပါ။

* **Ordered collection** - **Elements** တွေကို ထည့်လိုက်တဲ့ အစဉ်လိုက်အတိုင်းပဲ သိမ်းဆည်းပေးထားတာပါ။ ဒါကြောင့် သူ့ရဲ့ **Elements** တွေကို **Index** (Position) သုံးပြီး လှမ်းခေါ်လို့ ရပါတယ်။ 

* **Unordered collection** - **Elements** တွေကို ထည့်လိုက်တဲ့ အစဉ်လိုက်အတိုင်း သိမ်းမပေးပါဘူး။ ဒါကြောင့် **Element** တစ်ခုက ဘယ်နေရာ (Position) မှာ ရောက်နေမလဲဆိုတာ ကြိုခန့်မှန်းလို့ မရပါဘူး။ ဒီတော့ **Position** ကို အခြေခံတဲ့ **Index** ကိုသုံးပြီး လှမ်းခေါ်လို့ မရပါဘူး။

* **Sequence** - **Ordered collection** တွေကို ယေဘုယျခေါ်တဲ့ အခေါ်အဝေါ်ပါ။

* **Immutable** - ပြောင်းလဲလို့မရတဲ့ (**Unchangeable**) **Collection** ကို ဆိုလိုပါတယ်။ 

* **Mutable** - ပြောင်းလဲလို့ရတဲ့ (**Changeable**) **Collection** ကို ဆိုလိုပါတယ်။

အခုလေ့လာခဲ့ပြီးတဲ့ **Types** တွေက ဒီအချက်တွေထဲက ဘယ်ဟာတွေနဲ့ ကိုက်ညီလဲဆိုတာ ကြည့်လိုက်ရအောင် -

* **String** - **Ordered collection** ဖြစ်တယ်၊ **Immutable** ဖြစ်တယ်၊ **Iterable** ဖြစ်တယ်။

* **List** - **Ordered collection** ဖြစ်တယ်၊ **Mutable** ဖြစ်တယ်၊ **Iterable** ဖြစ်တယ်။

* **Tuple** - **Ordered collection** ဖြစ်တယ်၊ **Immutable** ဖြစ်တယ်၊ **Iterable** ဖြစ်တယ်။

* **Set** - **Unordered collection** ဖြစ်တယ်၊ **Mutable** ဖြစ်တယ်၊ **Iterable** ဖြစ်တယ်။

* **Dictionary** - **Unordered collection** ဖြစ်တယ်၊ **Mutable** ဖြစ်တယ်၊ **Iterable** ဖြစ်တယ်။

#### 3.5.2 Comments and Indentation

**Comments** တွေကို **#** နဲ့ စတင်ရေးသားရပါတယ်။

```python title="Comments begin with #"
# calculate gross salary 
gs = bs + da + hra + ca 
si = p * n * r / 100 # calculate simple interest
```

**Multi-line comments** တွေကို **'''** (သို့မဟုတ်) **"""** အစုံလိုက် (Pair) ကြားထဲမှာ ရေးသားသင့်ပါတယ်။

```python title="Multi-line comments example"
''' Additional program: Calculate bonus to be paid
URL: [https://github.com/Joseph1997-eng/Let-Us-Python-Book-](https://github.com/Joseph1997-eng/Let-Us-Python-Book-)
Author: Joseph, Date: 7 Dec 2025 '''
```

**Indentation** က အရမ်းအရေးကြီးပါတယ်! ပေါ့ပေါ့ဆဆ သုံးလို့မရပါဘူး။ အောက်က **Code** မှာဆိုရင် '**Unexpected indent**' ဆိုတဲ့ **Error** တက်ပါလိမ့်မယ်။

```python title="Indentation error example"
a = 20 
  b = 45 # ဘာ reason မှ မရှိဘဲ space ခွာထားလို့ Error တက်ပါမယ်
```

**Multi-lining**

တကယ်လို့ **Statements** တွေက ရှည်နေခဲ့ရင် စာကြောင်းအများကြီးခွဲပြီး (**Multi-lines**) ရေးလို့ရပါတယ်။ အဲဒီလိုရေးတဲ့အခါ နောက်ဆုံးစာကြောင်းကလွဲရင် ကျန်တဲ့စာကြောင်းတွေရဲ့ အဆုံးမှာ `\` ထည့်ပေးရပါမယ်။

```python title="Multi-lining"
total = physics + chemistry + maths + \
english + myanmar + history + \
geography + civics
```
`[ ]`၊ `{ }` (သို့မဟုတ်) `( )` တွေကြားထဲမှာရေးတဲ့ **Multi-line statements** တွေအတွက်တော့ `\` ထည့်ပေးစရာ မလိုပါဘူး။

```python title="Multi-line"
days = [ 'Monday', 'Tuesday', 'Wednesday', 'Thursday',
'Friday', 'Saturday', 'Sunday' ]
```

### 3.6 Classes and Objects

Python မှာ **Type** တိုင်းက **Class** တစ်ခု ဖြစ်ပါတယ်။ ဒါကြောင့် **int**၊ **float**၊ **complex**၊ **bool**၊ **str**၊ **list**၊ **tuple**၊ **set**၊ **dict** စတာတွေ အကုန်လုံးက **Classes** တွေချည်းပါပဲ။ ဒါတွေက **Ready-made classes** တွေပါ။ Python က **User-defined classes** တွေကို ကိုယ်တိုင်ဖန်တီးခွင့် ပေးထားပါတယ် (**Chapter 18** ကျရင် တွေ့ရပါမယ်)။

**Object** တစ်ခုကို **Class** ကနေ ဖန်တီးယူပါတယ်။ **Class** တစ်ခုက အချက်နှစ်ချက်ကို သတ်မှတ်ပေးပါတယ် -
1. သူ့ဆီကနေ ထွက်လာမယ့် **Object** ယူမယ့် ပုံစံ (**Form**)
2. အဲဒီ **Object** ကို **Access** လုပ်ဖို့နဲ့ **Manipulate** လုပ်ဖို့ သုံးရမယ့် **Methods** (**Functions**) များ



**Class** တစ်ခုတည်းကနေ **Objects** အများကြီး ဖန်တီးလို့ ရပါတယ်။ **Class** တစ်ခုကနေ **Object** တစ်ခု ဖန်တီးလိုက်တာကို အဲဒီ **Class** ရဲ့ **Instance** တစ်ခု ဖန်တီးလိုက်တယ်လို့ ပြောလေ့ရှိကြပါတယ်။

**Class** မှာ နာမည်ရှိပေမယ့် **Objects** တွေမှာ နာမည်မရှိပါဘူး။ **Objects** တွေမှာ နာမည်မရှိတဲ့အတွက် **Memory** ထဲက သူတို့ရဲ့ **Addresses** တွေကို သုံးပြီး ရည်ညွှန်း (**Refer**) ကြပါတယ်။

ဒီအချက်တွေကို အောက်ပါ **Program** နဲ့ စမ်းသပ်အတည်ပြုနိုင်ပါတယ်။ ပိုပြီးနားလည်သွားအောင် **Observation** (လေ့လာတွေ့ရှိချက်) တွေကို ကြည့်ပါ။

```python title="All the above statements can be verified through the following program."
a = 30
b = 'Good'
print(a, b) # 3 Good ဆိုပြီး print ထွက်ပါမယ်
print(type(a), type(b)) # <class 'int'> <class 'str'> ဆိုပြီး Class တွေကို ပြပါမယ်
print(id(a), id(b)) # 1356658640 33720000 ဆိုပြီး Memory address တွေ ပြပါမယ်
print(isinstance(a, int), isinstance(b, str)) # True True ဆိုပြီး ပြပါမယ်
```

### 3.7 Python Object Reference Visualization

Python မှာ **Variables** တွေက **Memory** ပေါ်မှာရှိတဲ့ **Objects** တွေကို ဘယ်လို **Refer** လုပ်သလဲ (ဘယ်လို ညွှန်ပြထားသလဲ) ဆိုတာ နားလည်ဖို့ အရမ်းအရေးကြီးပါတယ်။

!!! info "Key Concept"
    * Python မှာ **Variables** တွေဆိုတာ တကယ်တမ်းကျတော့ **Memory** ထဲမှာ သိမ်းဆည်းထားတဲ့ **Objects** တွေကို ညွှန်ပြနေတဲ့ **References** (သို့မဟုတ် **Pointers**) တွေပဲ ဖြစ်ပါတယ်။ သူတို့က **Values** တွေကို တိုက်ရိုက် သိမ်းဆည်းထားတာ မဟုတ်ပါဘူး။ **Value** သိမ်းထားတဲ့ **Memory location** ကို ညွှန်ပြပေးနေတာသာ ဖြစ်ပါတယ်။ 

## Memory Reference Breakdown

အောက်ပါဇယားက ပုံထဲမှာပြထားတဲ့ **References** တွေကို အသေးစိတ် ရှင်းပြထားတာပါ -

| Variable Name | Reference ID (Address) | Points To (Object Type) | Object Value | Object Memory Address |
| :--- | :--- | :--- | :--- | :--- |
| **`a`** | `1356658640` | **int object** | `30` | `1356658640` |
| **`b`** | `33720000` | **str object** | `Good` | `33720000` |

!!! note "Observation (လေ့လာတွေ့ရှိချက်)"
    * **Variable `a`** မှာ **Reference ID** `1356658640` ရှိနေပါတယ်။ အဲဒါက **Integer Object** `30` ရှိနေတဲ့ **Address** နဲ့ အတူတူပါပဲ။
    * **Variable `b`** မှာ **Reference ID** `33720000` ရှိနေပါတယ်။ အဲဒါက **String Object** `'Good'` ရှိနေတဲ့ **Address** နဲ့ အတူတူပါပဲ။

ဒီ **Program** မှာ ကျွန်တော်တို့ **Objects** နှစ်ခုကို ဖန်တီးခဲ့ပါတယ်။ တစ်ခုက **Ready-made class** ဖြစ်တဲ့ **int** ကနေဖြစ်ပြီး၊ နောက်တစ်ခုက **Ready-made class** ဖြစ်တဲ့ **str** ကနေ ဖြစ်ပါတယ်။

**int** type **Object** ထဲမှာ 30 ပါဝင်ပြီး၊ **str** type **Object** ထဲမှာတော့ 'Good' ပါဝင်ပါတယ်။

**Objects** နှစ်ခုလုံးက နာမည်မရှိပါဘူး (Nameless ဖြစ်ပါတယ်)။ **Memory** ထဲက သူတို့ရဲ့ **Addresses** တွေဖြစ်တဲ့ `1356658640` နဲ့ `33720000` ကို `a` နဲ့ `b` ထဲမှာ သိမ်းဆည်းထားတာပါ။

ဒီ **Addresses** တွေကို **Built-in function** ဖြစ်တဲ့ **id( )** ကိုသုံးပြီး ရယူနိုင်ပါတယ်။ (မှတ်ချက် - ခင်ဗျားတို့စက်မှာ ကိုယ်တိုင် Run ရင်တော့ **Addresses** တွေ မတူတာ ထွက်လာနိုင်ပါတယ်)။

`a` နဲ့ `b` က **Addresses** တွေကို သိမ်းထားတဲ့အတွက် သူတို့ကို အဲဒီ **Addresses** မှာရှိတဲ့ **Objects** တွေကို **Refer** လုပ်နေတယ် (ရည်ညွှန်းနေတယ်) လို့ ပြောကြပါတယ်။ လွယ်လွယ်ပြောရရင် သူတို့က **Objects** တွေကို ညွှန်ပြနေတဲ့ **Pointers** တွေပါပဲ။

`a` နဲ့ `b` က **Refer** လုပ်နေတဲ့ **Objects** တွေရဲ့ **Type** ကို သိချင်ရင် **Built-in function** ဖြစ်တဲ့ **type( )** ကို သုံးနိုင်ပါတယ်။

`a` က **class int** ရဲ့ **Instance** ဟုတ်မဟုတ် စစ်ဆေးချင်ရင်တော့ **Built-in function** ဖြစ်တဲ့ **isinstance( )** ကို သုံးနိုင်ပါတယ်။

**Multiple Objects**

အောက်ပါ **Program** လေးကို ဆက်ကြည့်ရအောင် -

```python title="Multiple Objects"
a = 3
b = 3
print(id(a), id(b)) # 1356658640 1356658640 ဆိုပြီး တူနေတာကို တွေ့ရပါမယ်
print(a is b) # True ပြပါမယ်
a = 30 # အခု a က Object အသစ်တစ်ခုကို Refer လုပ်သွားပါပြီ
print(id(a)) # 1356659072 ဆိုပြီး Address ပြောင်းသွားပါမယ်
```

ကျွန်တော်တို့ **int** objects နှစ်ခု ဖန်တီးလိုက်တာလား? မဟုတ်ပါဘူး။ **int** object ထဲမှာ သိမ်းထားတဲ့ **Value** က တူနေတဲ့အတွက် (နှစ်ခုလုံးက 3 ဖြစ်နေလို့)၊ **int** object တစ်ခုတည်းကိုပဲ ဖန်တီးပါတယ်။ `a` ရော `b` ရောက အဲဒီ **int** object တစ်ခုတည်းကိုပဲ လှမ်းပြီး **Refer** လုပ်နေကြတာပါ။ ဒါကြောင့် `id(a)` နဲ့ `id(b)` က တူညီတဲ့ **Addresses** တွေကို ပြန်ပေးတာဖြစ်ပါတယ်။ 

ဒါကို **is operator** သုံးပြီးလည်း စစ်ဆေးနိုင်ပါတယ်။ `a` နဲ့ `b` က **Object** တစ်ခုတည်းကိုပဲ **Refer** လုပ်နေတဲ့အတွက် `True` လို့ ပြန်ပေးပါလိမ့်မယ်။

ကျွန်တော်တို့က `a` ထဲကို **Value** အသစ်တစ်ခု ထည့်ဖို့ ကြိုးစားလိုက်တဲ့အခါ (ဥပမာ - 30 ထည့်လိုက်ရင်)၊ သိမ်းရမယ့် တန်ဖိုးက ကွဲပြားသွားပြီဖြစ်တဲ့အတွက် **int** object အသစ်တစ်ခုကို ဖန်တီးလိုက်ပါတယ်။ အခုအခါမှာ `a` က ဒီ **int** object အသစ်ကို ပြောင်းပြီး **Refer** လုပ်သွားပါပြီ။ `b` ကတော့ မူလ **int** object (Value 3 ရှိတဲ့ကောင်) ကိုပဲ ဆက်ပြီး **Refer** လုပ်နေတုန်းပါပဲ။

`a` က 3 ပါဝင်တဲ့ **int** object ကို **Refer** လုပ်နေတယ်လို့ ပြောမယ့်အစား၊ `a` သည် **int** object ဖြစ်တယ်၊ သို့မဟုတ် 3 ကို `a` ထဲ **Assign** လုပ်လိုက်တယ်လို့ပဲ အလွယ်ပြောလေ့ရှိကြပါတယ်။

**Programmers** တော်တော်များများက `a` နဲ့ `b` ကို **int variables** တွေ (တန်ဖိုးတွေကို တိုက်ရိုက်သိမ်းတဲ့ အကွက်တွေ) လို့ ထင်နေကြတုန်းပါပဲ။ တကယ်တမ်းက အဲဒီလိုမဟုတ်ဘူးဆိုတာ အခုလောက်ဆို သိလောက်ပါပြီ။

### Problem 3.1

**Integer types** တွေနဲ့ သူတို့အပေါ်မှာ သုံးလို့ရတဲ့ **Operators** တွေကို ဘယ်လိုအသုံးပြုမလဲဆိုတာ သရုပ်ပြပါ။

<details>
<summary>Program (နှိပ်ပြီး ကြည့်နိုင်ပါတယ်)</summary>

```python title="Problem 3.1"
# use of integer types
print(3 / 4)  # Division (အမြှောက်)
print(3 % 4)  # Modulus (အကြွင်း)
print(3 // 4) # Floor Division (စားလဒ် အရေအတွက်)
print(3 ** 4) # Exponentiation (ထပ်ကိန်း)

a = 10 ; b = 25 ; c = 15 ; d = 30 ; e = 2 ; f = 3 ; g = 5 
w = a + b - c 
x = d ** e 
y = f % g 
print(w, x, y)

# Python handles large integers automatically
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
    * **3/4** က 0 မထွက်ပါဘူး (Python 3 မှာ **Float division** ဖြစ်သွားလို့ 0.75 ထွက်ပါတယ်)။
    * တစ်ကြောင်းတည်းမှာ **Statements** အများကြီးရေးမယ်ဆိုရင် `;` ခံပြီး ခြားရေးရပါမယ်။
    * **print(w, x, y)** က **Values** တွေကို **Space** ခြားပြီး **Print** ထုတ်ပေးပါတယ်။

### Problem 3.2
**float**၊ **complex** နဲ့ **bool types** တွေနဲ့ သူတို့အပေါ်မှာ သုံးလို့ရတဲ့ **Operators** တွေကို ဘယ်လိုအသုံးပြုမလဲဆိုတာ သရုပ်ပြပါ။

<details>
<summary>Program (နှိပ်ပြီး ကြည့်နိုင်ပါတယ်)</summary>

```python title="Problem 3.2"
# use of float (float ကို အသုံးပြုခြင်း)
i = 3.5
j = 1.2
print(i % j) # Modulus ရှာခြင်း

# use of complex (complex number ကို အသုံးပြုခြင်း)
a = 1 + 2j
b = 3 * (1 + 2j)
c = a * b
print(a)
print(b)
print(c)
print(a.real) # Real part ကို ထုတ်ကြည့်ခြင်း
print(a.imag) # Imaginary part ကို ထုတ်ကြည့်ခြင်း
print(a.conjugate( )) # Conjugate လုပ်ခြင်း
print(a)

# use of bool (Boolean ကို အသုံးပြုခြင်း)
x = True
y = 3 > 4
print(x)
print(y)
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
    * `%` (Modulus operator) က **floats** တွေပေါ်မှာလည်း အလုပ်လုပ်ပါတယ်။
    * **Complex number** တစ်ခုကနေ **real** နဲ့ **imag** part တွေကို ခွဲထုတ်ယူလို့ရပါတယ်။
    * **Condition** တစ်ခုကို **Evaluation** လုပ်လိုက်ရင် **True** သို့မဟုတ် **False** အဖြစ် အစားထိုးသွားပါတယ်။


### Problem 3.3

**Number type** တစ်ခုကနေ နောက်တစ်ခုကို ဘယ်လို **Convert** လုပ်မလဲဆိုတာ သရုပ်ပြပါ။

<details>
<summary>Program (နှိပ်ပြီး ကြည့်နိုင်ပါတယ်)</summary>

```python title="Problem 3.3"
# convert to int (Integer ပြောင်းခြင်း)
print(int(3.14)) # float ကနေ int သို့ ပြောင်းတာပါ (ဒသမဖြတ်ပါတယ်)
a = int('485') # numeric string ကနေ int သို့
b = int('768') # numeric string ကနေ int သို့
c = a + b 
print(c)

# Base တွေပြောင်းပြီး int လုပ်ခြင်း
print(int('1011', 2)) # binary string ကနေ decimal int သို့ 
print(int('341', 8)) # octal string ကနေ decimal int သို့ 
print(int('21', 16)) # hex string ကနေ decimal int သို့ 

# convert to float (Float ပြောင်းခြင်း)
print(float(35)) # int ကနေ float သို့ (35.0 ဖြစ်သွားမယ်)
i = float('4.85') # numeric string ကနေ float သို့
j = float('7.68') # numeric string ကနေ float သို့
k = i + j 
print(k)

# convert to complex (Complex number ပြောင်းခြင်း)
print(complex(35)) # int ကနေ complex သို့ (35+0j)
x = complex(4.85, 1.1) # arguments နှစ်ခုပေးပြီး ဆောက်ခြင်း
y = complex(7.68, 2.1) 
z = x + y 
print(z)

# convert to bool (Boolean ပြောင်းခြင်း)
print(bool(35)) # Non-zero မို့ True ရပါမယ်
print(bool(1.2)) # Non-zero မို့ True ရပါမယ်
print(int(True)) # 1 ရပါမယ်
print(int(False)) # 0 ရပါမယ်
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
    * **Binary**, **Octal**, **Hexadecimal** numeric string တွေကို သူတို့နဲ့ညီမျှတဲ့ **Decimal integer** အဖြစ် ပြောင်းလို့ရပါတယ်။ ဒါပေမယ့် **Float** အတွက်တော့ အဲဒီလိုလုပ်လို့ မရပါဘူး။
    * **Complex** ကို Convert လုပ်တဲ့အခါ **Argument** တစ်ခုတည်းပေးမယ်ဆိုရင် **Imaginary part** ကို `0` လို့ ယူဆသွားပါတယ်။
    * သုညမဟုတ်တဲ့ ဂဏန်း (Non-zero number - int ဖြစ်ဖြစ် float ဖြစ်ဖြစ်) မှန်သမျှကို **True** လို့ သတ်မှတ်ပြီး၊ `0` ကိုတော့ **False** လို့ သတ်မှတ်ပါတယ်။

### Problem 3.4

**Built-in mathematical functions** တွေကို အသုံးပြုထားတဲ့ **Program** တစ်ပုဒ် ရေးပါ။

<details>
<summary>Program (နှိပ်ပြီး ကြည့်နိုင်ပါတယ်)</summary>

```python title="Problem 3.4"
# built-in math functions (ပါပြီးသား သင်္ချာ function များ)
print(abs(-25)) # Absolute value ရှာခြင်း (25)
print(pow(2, 4)) # ထပ်ကိန်းတင်ခြင်း (16)
print(min(10, 20, 30, 40, 50)) # အငယ်ဆုံးရှာခြင်း (10)
print(max(10, 20, 30, 40, 50)) # အကြီးဆုံးရှာခြင်း (50)
print(divmod(17, 3)) # စားလဒ်နဲ့ အကြွင်း တွဲထုတ်ခြင်း ((5, 2))
print(bin(64), oct(64), hex(64)) # Binary, Octal, Hex ပြောင်းခြင်း
print(round(2.567), round(2.5678, 2)) # ကိန်းပြည့်ဖြတ်ခြင်းနှင့် ဒသမ ၂ နေရာဖြတ်ခြင်း
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
    * **divmod(a, b)** က **(a // b, a % b)** ဆိုတဲ့ အတွဲ (**Pair**) ကို ထုတ်ပေးပါတယ်။
    * **bin( )**၊ **oct( )**၊ **hex( )** တွေက **Binary**၊ **Octal** နဲ့ **Hexadecimal** တန်ဖိုးတွေကို ပြန်ပေးပါတယ်။
    * **round(x)** ကို သုံးတဲ့အခါ ဒသမနေရာ မပါအောင် (**0 decimal places**) ဖြတ်မယ်လို့ ယူဆပြီး အလုပ်လုပ်ပါတယ်။

### Problem 3.5
**math module** ထဲက **Functions** တွေကို အသုံးပြုထားတဲ့ **Program** တစ်ပုဒ် ရေးပါ။

<details>
<summary>Program (နှိပ်ပြီး ကြည့်နိုင်ပါတယ်)</summary>

```python title="Problem 3.5"
# mathematical functions from math module
import math
x = 1.5357
print(math.pi, math.e) # pi နဲ့ e တန်ဖိုးများ
print(math.sqrt(x)) # Square root ရှာခြင်း
print(math.factorial(6)) # Factorial ရှာခြင်း
print(math.fabs(x)) # Absolute float value
print(math.log(x)) # Natural log (base e)
print(math.log10(x)) # Log base 10
print(math.exp(x)) # e raised to x
print(math.trunc(x)) # ဒသမဖြတ်ထုတ်ခြင်း (Truncate)
print(math.floor(x)) # အောက်ချခြင်း (Floor)
print(math.ceil(x)) # အပေါ်တင်ခြင်း (Ceiling)

# Negative values တွေနဲ့ စမ်းသပ်ခြင်း
print(math.trunc(-x))
print(math.floor(-x))
print(math.ceil(-x))

print(math.modf(x)) # Fractional part နဲ့ Integer part ကို ခွဲထုတ်ခြင်း
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
    * **floor( )** က **Negative infinity** ဘက်ကို ဆွဲချပြီး Round လုပ်ပါတယ် (တန်ဖိုးအနည်းဘက်ကို ယူပါတယ်)။ **ceil( )** က **Positive infinity** ဘက်ကို ဆွဲတင်ပြီး Round လုပ်ပါတယ် (တန်ဖိုးအများဘက်ကို ယူပါတယ်)။ **trunc( )** ကတော့ **0** ဘက်ကို ဦးတည်ပြီး Round လုပ်ပါတယ် (ဒသမတွေကို ရိုးရိုးလေး ဖြတ်ထုတ်လိုက်တာပါ)။ 
    * **Positive numbers** တွေအတွက်ဆိုရင် **trunc( )** က **floor( )** နဲ့ အတူတူပါပဲ။
    * **Negative numbers** တွေအတွက်ဆိုရင် **trunc( )** က **ceil( )** နဲ့ အတူတူပါပဲ။
    * **modf( )** က `(f, i)` ဆိုတဲ့ ကိန်းဂဏန်းအတွဲ (**Pair**) ကို ပြန်ပေးပါတယ် (ဒီမှာ `x = f + i` ဖြစ်ပြီး `0 <= f < 1` ဖြစ်ပါတယ်)။

### Problem 3.6

**Float** နဲ့ **Integer** **random numbers** တွေကို ထုတ်ပေးမယ့် **Program** တစ်ပုဒ် ရေးပါ။

<details>
<summary>Program (နှိပ်ပြီး ကြည့်နိုင်ပါတယ်)</summary>

```python title="Problem 3.6"
# random number operations using random module
import random 
import datetime

# Seed သတ်မှတ်ခြင်း (လက်ရှိအချိန်ကို မူတည်ပြီး Random ပုံစံပြောင်းအောင်လုပ်တာပါ)
# Note: ပုံမှန်အားဖြင့် Python က ဒါကို အလိုအလျောက် လုပ်ပေးပါတယ်
random.seed(datetime.time( )) 

print(random.random( )) # 0.0 နဲ့ 1.0 ကြား Random float
print(random.random( )) 
print(random.randint(10, 100)) # 10 နဲ့ 100 ကြား Random integer
```
</details>

<details>
<summary>Output</summary>

```python title="Output"
0.23796462709189137
0.5442292252959519
57
```
</details>

!!! note "Tips"
    * **random module** ကို မဖြစ်မနေ **import** လုပ်ဖို့ လိုအပ်ပါတယ်။
    * **Random number generation logic** ကို လက်ရှိအချိန် (Current time) နဲ့ **Seed** လုပ်ပေးလိုက်ရင်၊ **Program** ကို **Execute** လုပ်လိုက်တိုင်း မတူညီတဲ့ **Random numbers** တွေကို ရရှိစေပါတယ်။
    * **Parameter** မပါတဲ့ **random.seed( )** ကလည်း **Logic** ကို လက်ရှိအချိန်နဲ့ပဲ **Seed** လုပ်ပေးပါတယ်။

### Problem 3.7

အောက်ဖော်ပြပါ Data တွေထဲက ဘယ်ဟာက **string**၊ **list**၊ **tuple**၊ **set** (သို့မဟုတ်) **dictionary** ဖြစ်မလဲဆိုတာ ဘယ်လို ခွဲခြားသိနိုင်မလဲ?

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
# determine type of data (Data Type တွေကို စစ်ဆေးခြင်း)
print(type({10, 20, 30.5})) # Curly braces {} နဲ့မို့ Set ပါ
print(type([1, 2, 3.14, 'Nagpur'])) # Square brackets [] နဲ့မို့ List ပါ
print(type({12 : 'Simple', 43 : 'Complicated', 13 : 'Complex'})) # Key-Value pairs ပါလို့ Dict ပါ
print(type("Check it out!")) # Quotes "" ပါလို့ String ပါ
print(type(3 + 2j)) # j ပါလို့ Complex ပါ
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
    * **type( )** ဆိုတာက **built-in** ဖြစ်စေ၊ **container** ဖြစ်စေ၊ **user-defined** ဖြစ်စေ မည်သည့် **Data** အမျိုးအစားကိုမဆို ခွဲခြားစစ်ဆေးပေးနိုင်တဲ့ **Built-in function** တစ်ခုဖြစ်ပါတယ်။

## **Exercises**

### **[A] Answer the following questions:**

**a.** Variable `a` နဲ့ `b` ရဲ့ တန်ဖိုးတွေကို အချင်းချင်းလှဲလှယ် (**Swap**) ပေးမယ့် Program တစ်ပုဒ်ရေးပါ။ တတိယ **Variable** တစ်လုံးကို အကူအညီယူပြီး သုံးခွင့်မရှိပါဘူး။ `a` နဲ့ `b` အပေါ်မှာ **Arithmetic operations** (အပေါင်း၊ အနုတ် စသည်) လုပ်ဆောင်ခွင့်မရှိပါဘူး။

**b.** **math module** မှာပါဝင်တဲ့ **Trigonometric functions** တွေကို အသုံးပြုထားတဲ့ Program တစ်ပုဒ်ရေးပါ။

**c.** 10 ကနေ 50 ကြားထဲမှာရှိတဲ့ **Random numbers** 5 လုံးကို ထုတ်ပေးမယ့် Program တစ်ပုဒ်ရေးပါ။ **Seed value** ကို 6 ထားပြီး သုံးပါ။ Program ကို **Execute** လုပ်လိုက်တိုင်း ဒီ **Seed value** ကို **Execution time** နဲ့ တွဲပြီး ပြောင်းလဲသွားအောင် (**Change** ဖြစ်သွားအောင်) စီစဉ်ပေးပါ။

**d.** -2.8, -0.5, 0.2, 1.5 နဲ့ 2.9 စတဲ့ ကိန်းဂဏန်းတွေအတွက် **trunc( )**၊ **floor( )** နဲ့ **ceil( )** တို့ရဲ့ ကွာခြားချက်ကို ရှင်းရှင်းလင်းလင်း သိရအောင် လက်တွေ့စမ်းသပ်ပါ။

**e.** မြို့တစ်မြို့ရဲ့ အပူချိန်ကို **Fahrenheit degrees** နဲ့ သင့်တော်သလို သတ်မှတ်ပါ။ ပြီးရင် ဒီအပူချိန်ကို **Centigrade degrees** ပြောင်းလဲပြီး အပူချိန်နှစ်မျိုးလုံးကို **Print** ထုတ်ပေးမယ့် Program ရေးပါ။

**f.** တြိဂံတစ်ခုရဲ့ အနားများဖြစ်တဲ့ `a`, `b`, `c` တို့ကို ပေးထားရင်၊ ယင်းတြိဂံရဲ့ ထောင့် (Angles) ၃ ခုကို ရှာဖွေပြီး **Next integer** အဖြစ် **Round** လုပ်ကာ ထုတ်ပေးမယ့် Program ကို ရေးပါ။ အောက်ပါ **Formulae** များကို အသုံးပြုပါ -

$$ a^2 = b^2 + c^2 - 2bc.cos A, b^2 = a^2 + c^2 - 2ac.cos B, c^2 = a^2 + b^2 - 2ab.cos C$$


### **[B] How will you perform the following operations:**

အောက်ပါ **Operations** တွေကို ဘယ်လို လုပ်ဆောင်မလဲ -

**a.** `2 + 3j` ရဲ့ **Imaginary part** ကို Print ထုတ်ပါ။

**b.** `4 + 2j` ရဲ့ **Conjugate** ကို ရယူပါ။

**c.** **Binary** `1100001110` နဲ့ ညီမျှတဲ့ **Decimal** တန်ဖိုးကို Print ထုတ်ပါ။

**d.** **Float value** `4.33` ကို **Numeric string** အဖြစ် ပြောင်းလဲပါ။

**e.** `29` ကို `5` နဲ့ စားတဲ့အခါ ရလာမယ့် **Integer quotient** (ကိန်းပြည့်စားလဒ်) နဲ့ **Remainder** (အကြွင်း) ကို ရယူပါ။

**f.** **Decimal** `34567` နဲ့ ညီမျှတဲ့ **Hexadecimal** တန်ဖိုးကို ရယူပါ။

**g.** `45.6782` ကို ဒသမ ၂ နေရာအထိ (**Second decimal place**) **Round-off** လုပ်ပါ။

**h.** `3.556` ကနေ **4** ရအောင် လုပ်ပါ။ (Hint: `ceil` သို့မဟုတ် `round`)

**i.** `16.7844` ကနေ **17** ရအောင် လုပ်ပါ။

**j.** `3.45` ကို `1.22` နဲ့ စားတဲ့အခါ ရလာမယ့် **Remainder** (အကြွင်း) ကို ရယူပါ။

### **[C] Which of the following is invalid variable name and why?**

အောက်ဖော်ပြပါအမည်တွေထဲက ဘယ်ဟာက **Invalid variable name** (မှားယွင်းနေတဲ့ နာမည်) ဖြစ်သလဲ၊ ဘာကြောင့်လဲ?

|BASICSALARY | _basic | basic-hra|#MEAN|
|---|---|---|---|
|group.|422|pop in 2020|over|
|timemindovermatter|SINGLE|hELLO|queue.|
|team'svictory | Plot#3 | 2015_DDay||

### **[D] Evaluate the following expressions:**

အောက်ပါ **Expressions** တွေကို **Evaluate** လုပ်ပါ (တွက်ချက်အဖြေထုတ်ပါ) -
(မှတ်ချက် - **Operator Precedence** ခေါ် ဦးစားပေးအဆင့်ကို သတိပြုတွက်ချက်ပါ)



**a.** `2 ** 6 // 8 % 2`

**b.** `9 ** 2 // 5 - 3`

**c.** `10 + 6 - 2 % 3 + 7 - 2`

**d.** `5 % 10 + 10 -23 * 4 // 3`

**e.** `5 + 5 // 5 - 5 * 5 ** 5 % 5`

**f.** `7 % 7 + 7 // 7 - 7 * 7`


### **[E] Evaluate the following expressions:**

အောက်ပါ **Expressions** တွေကို **Evaluate** လုပ်ပါ -

**a.** `min(2, 6, 8, 5)`

**b.** `bin(46)`

**c.** `round(10.544336, 2)`

**d.** `math.hypot(6, 8)`

**e.** `math.modf(3.1415)`


### **[F] Match the following pairs:**

အောက်ပါ အတွဲများကို မှန်ကန်အောင် ယှဉ်တွဲပေးပါ -

| Column A | Column B |
|---|---|
| a. complex | 1. `\` |
| b. Escape special character | 2. Container type |
| c. Tuple | 3. Basic type |
| d. Natural logarithm | 4. log( ) |
| e. Common logarithm | 5. log10( ) |



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
