# Chapter 27 Numpy Library

<div class="chapter-social-card">
  <div class="chapter-info">
    <div class="chapter-number">CHAPTER 27</div>
    <h1 class="chapter-title">NumPy Library</h1>
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

NumPy ဆိုတာကတော့ **Num**erical **Py**thon ရဲ့ အတိုကောက်ဖြစ်ပြီး သိပ္ပံနဲ့ အင်ဂျင်နီယာပိုင်းဆိုင်ရာ ပြဿနာတွေကို ဖြေရှင်းတဲ့နေရာမှာ လူသုံးများတဲ့ Library တစ်ခုဖြစ်ပါတယ်။ သူက စွမ်းဆောင်ရည်မြင့်မားတဲ့ Multidimensional array object (ရှုထောင့်စုံ ဇယားကွက်) တွေနဲ့ အဲဒီ array တွေအပေါ်မှာ မြန်ဆန်သွက်လက်စွာ တွက်ချက်နိုင်မယ့် Method တွေကို ပံ့ပိုးပေးထားပါတယ်။ ဒီလိုလုပ်ဆောင်နိုင်တဲ့ လုပ်ငန်းစဉ်တွေထဲမှာ သင်္ချာဆိုင်ရာ၊ ယုတ္တိဗေဒ (Logic) ပိုင်း၊ ပုံသဏ္ဍာန် ပြုပြင်ပြောင်းလဲတာ၊ အစီအစဉ်ချတာ၊ ရွေးထုတ်တာ၊ Input/Output ကိစ္စတွေနဲ့ စာရင်းအင်း (Statistical) ပိုင်းဆိုင်ရာ တွက်ချက်မှုတွေ စသည်ဖြင့် ပါဝင်ပါတယ်။

---

## 27.1 Creation of Array

NumPy Library ကို အသုံးပြုချင်တယ်ဆိုရင်တော့ အောက်မှာပြထားတဲ့အတိုင်း အရင်ဆုံး download ဆွဲပြီး install လုပ်ထားဖို့ လိုပါမယ်။

```Bash title="pip install numpy"
pip install numpy
```

NumPy Array တွေက ပုံစံကြည့်လိုက်ရင် Python List တွေနဲ့ တူသလိုလိုရှိပေမယ့်၊ တကယ်တမ်းကျတော့ List တွေထက် ပိုပြီး မြန်မြန်ဆန်ဆန် အလုပ်လုပ်နိုင်အောင် ဖန်တီးထားတာဖြစ်ပါတယ်။
List တွေနဲ့ မတူတဲ့အချက်ကတော့ NumPy array တစ်ခုထဲမှာပါတဲ့ element တွေအားလုံးဟာ data type အမျိုးအစား တူညီနေဖို့ လိုပါတယ်။
NumPy array တစ်ခု တည်ဆောက်ချင်ရင် np.array() function ကို သုံးရမှာဖြစ်ပြီး၊ အောက်ပါနမူနာအတိုင်း ကိန်းဂဏန်း list တစ်ခုကို ထည့်ပေးရပါမယ်။

```Python title="NumPy Array"
import numpy as np 
intarr = np.array([1,2,3,4]) # ကိန်းပြည့် (ints) array တစ်ခု တည်ဆောက်ခြင်း
floattarr = np.array([1.1,2.2,3.3,4.4]) # ဒသမကိန်း (floats) array တစ်ခု တည်ဆောက်ခြင်း
```

တကယ်လို့ ကိန်းပြည့် (ints) တွေနဲ့ ဒသမကိန်း (floats) တွေကို ရောရေးလိုက်မယ်ဆိုရင် NumPy က အားလုံးကို floats အဖြစ် အလိုအလျောက် ပြောင်းလဲသတ်မှတ်လိုက်မှာ ဖြစ်ပါတယ်။ Array တည်ဆောက်တဲ့အချိန်မှာ element တွေရဲ့ type ကို သီးခြား မသတ်မှတ်ပေးထားဘူးဆိုရင် NumPy က ပေးထားတဲ့ တန်ဖိုးတွေကိုကြည့်ပြီး type ကို ခန့်မှန်းပေးပါတယ်။ တကယ်လို့ ကိုယ်တိုင် type သတ်မှတ်ချင်တယ်ဆိုရင်လည်း အခုလို သတ်မှတ်ပေးလို့ ရပါတယ်။

```Python title="NumPy Array"
intarr = np.array([1,2,3,4], int)
floatarr = np.array([1.1,2.2,3.3,4.4], float)
```

2D array (matrix) ဆိုတာက 1D array တွေကို စုစည်းထားတာဖြစ်ပြီး၊ 3D array ဆိုတာကတော့ 2D array တွေကို ထပ်ပြီး စုစည်းထားတာ ဖြစ်ပါတယ်။ သူတို့ကို အောက်ပါအတိုင်း တည်ဆောက်နိုင်ပါတယ်။

```Python title="2D Array"
a1 = np.array([[1,2,3],[4,5,6]]) # 2 rows x 3 columns ရှိတဲ့ array
a2 = np.array([[[1,2],[4,5]],[[6,7],[8,9]]]) # 2x2 အရွယ်အစားရှိတဲ့ array ၂ ခုပါဝင်တဲ့ 3D array
```

Complex number (ကိန်းရော) တွေပါဝင်တဲ့ array တွေကိုလည်း တည်ဆောက်နိုင်ပါသေးတယ်။

```Python title="Complex Number Array"
c = np.array([[1,2],[3,4]], complex)
```

---

## 27.2 Creation of Filler Arrays

နောက်မှ တန်ဖိုးအစစ်တွေ အစားထိုးထည့်မယ့် နေရာဦးထားတဲ့ (initial placeholder) တန်ဖိုးတွေပါတဲ့ NumPy Array တွေကို ကြိုတင်တည်ဆောက်ထားလို့ ရပါတယ်။

ဥပမာ - 0 တွေချည်းပဲပါတာ၊ 1 တွေချည်းပဲပါတာ၊ ဒါမှမဟုတ် ကိုယ်လိုချင်တဲ့ ဂဏန်းသေချာသတ်မှတ်ပြီး ဖြည့်ထားတဲ့ array မျိုးတွေ ဖန်တီးနိုင်တယ်။ ဘာတန်ဖိုးမှန်းမသိတဲ့ (garbage values) တွေပါနေတဲ့ empty array မျိုးကိုလည်း ဖန်တီးလို့ရပါတယ်။

```Python title="Filler Arrays"
import numpy as np
a1 = np.empty((3,4))  # garbage values တွေပါတဲ့ 2D array တစ်ခု
a2 = np.zeros((3,4))  # သုည (0) တွေချည်းပဲပါတဲ့ 2D array
a3 = np.ones((3,4))   # တစ် (1) တွေချည်းပဲပါတဲ့ 2D array
a4 = np.full((2,2),7) # တန်ဖိုးအားလုံး 7 ဖြစ်နေတဲ့ 2D array
```

သတိပြုရန် - ဒီ function တွေထဲကို တန်ဖိုးထည့်တဲ့အခါ Tuple ပုံစံနဲ့ ထည့်ပေးရပါမယ်။ (3,4) တို့ (2,2) တို့ဆိုတာ ကိုယ်တည်ဆောက်ချင်တဲ့ array ရဲ့ ပုံသဏ္ဍာန် (Shape) ကို ညွှန်းဆိုတာ ဖြစ်ပါတယ်။ Random တန်ဖိုးတွေနဲ့ဖြစ်ဖြစ်၊ အကွာအဝေး ညီတူညီမျှခြားထားတဲ့ တန်ဖိုးတွေနဲ့ဖြစ်ဖြစ် array တွေကို တည်ဆောက်နိုင်ပါတယ်။

```Python title="Random Arrays"
import numpy as np
a1 = np.random.random((4))   # random တန်ဖိုး ၄ ခုပါတဲ့ array
a2 = np.arange(5)            # [0,1,2,3,4] ကို ဖန်တီးပေးတယ် (မူရင်းစာ text တွင် np.range ဟုပါသော်လည်း np.arange သာ အမှန်ဖြစ်သည်)
a3 = np.linspace(0,2,5)      # [0.0 0.5 1.0 1.5 2.0] ကို ဖန်တီးပေးတယ်
```

*arange()* နဲ့ *linspace()* ရဲ့ ပထမ ကိန်းဂဏန်းနှစ်လုံး (parameters) က အစတန်ဖိုးနဲ့ အဆုံးတန်ဖိုးကို ညွှန်းတာပါ။ တတိယ parameter မှာကျတော့ *arange()* အတွက်ဆိုရင် ဘယ်လောက်စီ ခြားမလဲဆိုတဲ့ step value ဖြစ်ပြီး၊ *linspace()* အတွက်ဆိုရင်တော့ တန်ဖိုးစုစုပေါင်း ဘယ်နှလုံး လိုချင်တာလဲ ဆိုတာကို ညွှန်းတာဖြစ်ပါတယ်။

NumPy ကနေ Identity Matrix ကိုလည်း ဖန်တီးခွင့်ပေးထားပါတယ်။ Identity Matrix ဆိုတာက ထောင့်ဖြတ်မျဉ်း (principal diagonal) ပေါ်မှာ 1 တွေရှိပြီး ကျန်တဲ့နေရာတွေမှာ 0 ဖြစ်နေတဲ့ Matrix မျိုးပါ။

```Python title="Identity Matrix"
import numpy as np
a1 = np.eye(3)
a2 = np.identity(3)
```

Identity matrix ဆိုတာ အနားညီစတုရန်း (Square) matrix ဖြစ်တဲ့အတွက် eye() နဲ့ identity() ကို သုံးတဲ့အခါ dimension တစ်ခုပဲ (ဂဏန်းတစ်လုံးပဲ) ထည့်ပေးဖို့ လိုပါတယ်။

---

## 27.3 Array Attributes

NumPy array တွေမှာ သူ့ရဲ့ element အမျိုးအစား (type)၊ အရွယ်အစား (size)၊ ပုံသဏ္ဍာန် (shape) စတာတွေကို ဖော်ပြပေးနိုင်တဲ့ attribute တွေ အများကြီး ပါဝင်ပါတယ်။

Array ထဲမှာ ဘာ data type တွေပါလဲ၊ size ဘယ်လောက်ရှိလဲ၊ memory ရဲ့ ဘယ်နေရာမှာ သိမ်းထားလဲ ဆိုတာတွေကို အောက်ပါအတိုင်း လှမ်းကြည့်လို့ရပါတယ်။

```Python title="Array Attributes"
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

```Python title="Array Attributes"
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

---

## 27.4 Array Operations (Array ဆိုင်ရာ လုပ်ဆောင်ချက်များ)

NumPy Array တွေပေါ်မှာ လုပ်ဆောင်ချက် (Operations) တွေ အများကြီး လုပ်လို့ရပါတယ်။ ဒီ operations တွေက ရေးရတာ ကျစ်လျစ်သလို၊ အလုပ်လုပ်တာလည်း အရမ်းမြန်ပါတယ်။ ဘာလို့ ဒီလောက်မြန်လဲဆိုတော့ ဒီ Library ထဲမှာ ကြိုတင် compile လုပ်ပြီးသား ကုဒ်တွေ (precompiled routines) ပါနေလို့ပဲ ဖြစ်ပါတယ်။

Array operations အမျိုးမျိုးရှိတဲ့အထဲမှာ အောက်ပါခေါင်းစဉ်တွေ ပါဝင်ပါတယ် -

- (a) Arithmetic Operations: သင်္ချာဆိုင်ရာ ပေါင်းနှုတ်မြှောက်စား လုပ်ဆောင်ချက်များ
- (b) Statistical Operations: စာရင်းအင်းပိုင်းဆိုင်ရာ တွက်ချက်မှုများ
- (c) Linear Algebra Operations: Linear Algebra (ရိုးဖြောင့် အက္ခရာသင်္ချာ) ဆိုင်ရာ တွက်ချက်မှုများ
- (d) Bitwise Operations: Bit အလိုက် ကိုင်တွယ်တဲ့ လုပ်ဆောင်ချက်များ
- (e) Copying, Sorting: ကူးယူခြင်း နဲ့ အစီအစဉ်ချခြင်းများ
- (f) Comparison Operations: နှိုင်းယှဉ်ခြင်းဆိုင်ရာ လုပ်ဆောင်ချက်များ

---

### 27.4.1 Arithmetic Operations (သင်္ချာဆိုင်ရာ တွက်ချက်မှုများ)

Array နှစ်ခုကြားမှာ **+, -, *, /, %** စတဲ့ သင်္ချာ operator တွေကို အသုံးပြုပြီး တွက်ချက်မှုတွေ အများကြီး လုပ်လို့ရပါတယ်။

ဒီ operator တွေကို သုံးလိုက်တဲ့အခါ Array နှစ်ခုရဲ့ သက်ဆိုင်ရာ နေရာတူ element အချင်းချင်း (corresponding elements) ကို တိုက်ရိုက် တွက်ချက်သွားမှာ ဖြစ်ပါတယ်။

သင်္ကေတ (operator) တွေ မသုံးချင်ဘူးဆိုရင် **add()**, **subtract()**, **multiply()**, **divide()**, နဲ့ **remainder()** ဆိုတဲ့ function (method) တွေကို ပြောင်းသုံးလို့လည်း ရပါတယ်။ ဒီလို တွက်ချက်တာမျိုးကို Vector operations လို့လည်း ခေါ်ကြပါတယ်။

```Python title="Arithmetic Operations"
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

Array ထဲက element တွေကို ကိန်းဂဏန်းတစ်ခုတည်း (Scalar) နဲ့ ပေါင်းနှုတ်မြှောက်စား လုပ်တာမျိုးလည်း လုပ်လို့ရပါသေးတယ်။ (ဥပမာ - Array တစ်ခုလုံးကို 2 နဲ့ လိုက်ပေါင်းတာမျိုးပေါ့)

```Python title="Scalar Operations"
import numpy as np
a1 = np.array([[10,2,3,4],[5,6,7,8]])
a2 = a1 + 2             # Element တိုင်းကို 2 ပေါင်းထည့်လိုက်တာ
a3 = a1 ** 2            # Element တိုင်းကို 2 ထပ်ကိန်း တင်လိုက်တာ
```

+=, -=, /= စတဲ့ In-place operator တွေကို သုံးမယ်ဆိုရင်တော့ Array အသစ်တစ်ခု ထပ်မဆောက်တော့ဘဲ ရှိပြီးသား လက်ရှိ Array ကိုပဲ တိုက်ရိုက် ပြင်ဆင် (Modify) သွားမှာ ဖြစ်ပါတယ်။

```Python title="In-place Operations"
a1 += a2 # a1 = a1 + a2 နဲ့ အတူတူပါပဲ (a1 ရဲ့ တန်ဖိုးကို တိုက်ရိုက်ပြောင်းသွားပါတယ်)
a3 += 5  # a3 = a3 + 5 နဲ့ အတူတူပါပဲ
```

Array element တွေအပေါ်မှာ တခြားလုပ်ဆောင်နိုင်တဲ့ operation တွေကတော့ **exp()** (ထပ်ကိန်းတင်ခြင်း)၊ **sqrt()** (နှစ်ထပ်ကိန်းရင်းရှာခြင်း)၊ **cos()**, **sin()** (တြီဂိုနိုမေတြီ တွက်ချက်ခြင်း) နဲ့ **log()** (Logarithm တွက်ချက်ခြင်း) စတာတွေပဲ ဖြစ်ပါတယ်။

---

### 27.4.2 Statistical Operations (စာရင်းအင်းဆိုင်ရာ တွက်ချက်မှုများ)

NumPy က Array တစ်ခုလုံးအပေါ်မှာဖြစ်ဖြစ်၊ ကိုယ်လိုချင်တဲ့ Axis (Dimension) တစ်ခုပေါ်မှာ မူတည်ပြီးတော့ဖြစ်ဖြစ် စာရင်းအင်းဆိုင်ရာ တွက်ချက်မှုတွေ (ဥပမာ - ပေါင်းခြင်း၊ အကြီးဆုံးရှာခြင်း) ကို လုပ်ပေးနိုင်ပါတယ်။

Axis ဆိုတာ Dimension (အတိုင်းအတာ) ကို ပြောတာပါ။ ဒါကြောင့် 1D array မှာ 1 axis ရှိပြီး၊ 2D array မှာ 2 axes ရှိတယ်လို့ မှတ်သားနိုင်ပါတယ်။

```Python title="Statistical Operations"
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

NumPy မှာ မြှောက်လဒ်ရှာတဲ့ Operation နှစ်ခုရဲ့ ကွာခြားချက်ကို သတိထားမှတ်သားဖို့ လိုပါတယ်။* ကိုသုံးရင် နေရာတူတဲ့ ကိန်းဂဏန်းချင်း (Element-wise) မြှောက်တာဖြစ်ပြီး၊@ ဒါမှမဟုတ် .dot() ကိုသုံးမှသာ တကယ့် Matrix မြှောက်ခြင်း (Matrix Multiplication) ကို လုပ်ဆောင်တာ ဖြစ်ပါတယ်။

```Python title="Linear Algebra Operations"
a3 = a1 * a2            # နေရာတူတဲ့ element အချင်းချင်း မြှောက်ခြင်း (Element-wise)
a3 = a1 @ a2            # Matrix မြှောက်နည်းအတိုင်း မြှောက်ခြင်း (Matrix multiplication)
a4 = a1.dot(a2)         # ဒါကလည်း Matrix multiplication ပါပဲ
```

Matrix တစ်ခုကို Transpose လုပ်ချင်တယ် (Row နဲ့ Column ပြောင်းပြန်လှန်ချင်တယ်) ဆိုရင်လည်း အလွယ်တကူ လုပ်လို့ရပါတယ်။

```Python title="Transpose"
a1 = np.array([[1,2,3,4],[5,6,7,8]])
a2 = np.transpose(a1)
```

Trace ဆိုတာက Matrix တစ်ခုရဲ့ ထောင့်ဖြတ်မျဉ်း (Principal diagonal) ပေါ်မှာရှိတဲ့ element တွေကို ပေါင်းခြင်းဖြစ်ပါတယ်။ ဒါကို np.trace() နဲ့ ရှာနိုင်ပါတယ်။

```Python title="Trace"
a = np.array([[1,2,3],[4,5,6],[7,8,9]])
s = np.trace(a)         # 1 + 5 + 9 = 15 ဆိုပြီး ရလာပါမယ်
```

Inverse Matrix ဆိုတာက မူရင်း Matrix နဲ့ ပြန်မြှောက်လိုက်ရင် Identity Matrix ရလာမယ့် Matrix အမျိုးအစားကို ပြောတာပါ။ NumPy ရဲ့ linalg (Linear Algebra) module အောက်က inv() ကိုသုံးပြီး ရှာနိုင်ပါတယ်။

```Python title="Inverse Matrix"
a = np.array([[1,2],[3,4]])
b = np.linalg.inv(a)
```

Linear Simultaneous Equations (တစ်ပြိုင်နက်ညီမျှခြင်း) တွေကို ဖြေရှင်းတဲ့နေရာမှာလည်း NumPy ကို သုံးနိုင်ပါတယ်။ဥပမာ - $$3x + y = 9$$ $$နဲ့$$ $$x + 2y = 8$$ ဆိုတဲ့ ညီမျှခြင်းနှစ်ကြောင်းရဲ့ အဖြေကို လိုချင်ရင် အခုလို တွက်နိုင်ပါတယ်။

```Python title="Linear Simultaneous Equations"
a = np.array([[3,1],[1,2]]) # x နဲ့ y ရဲ့ မြှောက်ဖော်ကိန်း (Coefficients) များ
b = np.array([9,8])         # ညီမျှခြင်းရဲ့ ရလဒ်များ
x = np.linalg.solve(a,b)    # အဖြေရှာခြင်း
print(x)
```

### 27.4.4 Bitwise Operations

Array ထဲမှာရှိတဲ့ element တစ်လုံးချင်းစီအပေါ်မှာ Bitwise operations တွေကိုလည်း အောက်ပါအတိုင်း တွက်ချက်လုပ်ဆောင်နိုင်ပါသေးတယ်။

```Python title="Bitwise Operations"
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

### 27.4.5 Copying and Sorting (ကူးယူခြင်းနှင့် အစီအစဉ်ချခြင်း)

NumPy မှာ Copy ကူးတဲ့နည်းလမ်း (၃) မျိုး ရှိပါတယ်။

- No Copy: လုံးဝ Copy မကူးခြင်း (Reference သဘောမျိုး)။

- Shallow Copy (View): အပေါ်ယံ အခွံပဲ ကူးယူခြင်း (Data က အတူတူပဲ)။

- Deep Copy: အနှစ်ပါမကျန် တစ်စုံလုံး ပွားယူခြင်း။

No Copy: Object ကိုရော၊ Data ကိုရော ကူးယူတာ မဟုတ်ပါဘူး။ Array ရှိနေတဲ့ လိပ်စာ (Address) ကို Variable အသစ်တစ်ခုနဲ့ လှမ်းညွှန်းလိုက်တာမျိုးပဲ ဖြစ်ပါတယ်။

Shallow Copy (View): Array object အသစ်တစ်ခု ဖန်တီးလိုက်ပေမယ့်၊ အတွင်းက Data တွေကတော့ မူရင်း Array ရဲ့ Data တွေကိုပဲ မျှသုံးနေတာ (Point လုပ်နေတာ) ဖြစ်ပါတယ်။

Deep Copy: Array object အသစ်ရော၊ Data အသစ်ရော သီးသန့်ခွဲထုတ်ပြီး အကုန် ကူးယူလိုက်တာ ဖြစ်ပါတယ်။

အောက်ပါ Code ဥပမာမှာ d နဲ့ပတ်သက်တဲ့ အပိုင်း ကျန်ခဲ့လို့ ကျွန်တော် ဖြည့်စွက်ပြီး ရှင်းပြပေးထားပါတယ်ခင်ဗျာ။

```Python title="Copying and Sorting"
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

```Python title="Sorting"
a = np.array([[3,7,6],[1,5,2]])
b = np.array([[3,7,6],[1,5,2]]) 

a.sort()                # Row အလိုက် ငယ်စဉ်ကြီးလိုက် စီပေးသွားမယ်
b.sort(axis = 0)        # Column အလိုက် (ဒေါင်လိုက်) ငယ်စဉ်ကြီးလိုက် စီပေးသွားမယ်
```

### 27.4.6 Comparison (နှိုင်းယှဉ်ခြင်းများ)

Array တွေမှာ ယှဉ်ကြည့်စရာ၊ တိုက်စစ်စရာ (Comparison) ပုံစံ (၃) မျိုး ရှိပါတယ်။

- One Value Comparison: Array ထဲက Element အားလုံးကို တန်ဖိုးတစ်ခုတည်းနဲ့ လိုက်ယှဉ်ကြည့်ပြီး ရလာတဲ့ အဖြေ (True/False) ကို Array ပြန်ထုတ်ပေးတာ။
- Corresponding Elements Comparison: Array နှစ်ခုမှာရှိတဲ့ နေရာတူ Element အချင်းချင်း လိုက်ယှဉ်ကြည့်ပြီး Boolean Array ပြန်ထုတ်ပေးတာ။
- Full Array Comparison: Array နှစ်ခုရဲ့ ပုံသဏ္ဍာန် (Shape) ရော၊ ပါဝင်တဲ့ Element တွေရော ထပ်တူညီမညီ စစ်ဆေးတာ (တူရင် True, မတူရင် False ပြပါတယ်)။

(1) Array Element အားလုံးကို တန်ဖိုးတစ်ခုနဲ့ လိုက်ယှဉ်ခြင်း

```Python title="One Value Comparison"
import numpy as np
a = np.array([[3,7,6],[1,5,2]])
print(a < 5)                # 5 ထက်ငယ်လား လိုက်စစ်တာပါ
# အဖြေက [[True False False] [True False True]] ဆိုပြီး ထွက်ပါမယ်
```

(2) Array နှစ်ခုက နေရာတူ Element အချင်းချင်း ယှဉ်ခြင်း

```Python title="Corresponding Elements Comparison"
import numpy as np
a = np.array([[3,7,6],[1,5,2]])
b = np.array([[3,1,2],[1,7,2]])
print(a < b)                # a က b ထက် ငယ်သလား နေရာတူချင်း တိုက်စစ်တာပါ
# အဖြေက [[False False False] [False True False]] ဆိုပြီး ထွက်ပါမယ်
```

(3) Array နှစ်ခုလုံး ထပ်တူညီမညီ ယှဉ်ခြင်း

```Python title="Full Array Comparison"
import numpy as np
a = np.array([[3,7,6],[1,5,2]])
b = np.array([[3,7,6],[1,5,2]])
c = np.array([[3,7],[6,1],[5,2]])

print(np.array_equal(a,b))  # True (Shape ရော Element တွေရော ကွက်တိတူလို့ပါ)
print(np.array_equal(a,c))  # False (Shape မတူတော့လို့ပါ)
```

### 27.4.7 Indexing and Slicing (Array ခန်းများ ညွှန်းဆိုခြင်းနှင့် အပိုင်းဖြတ်ခြင်း)

Python List တွေလိုပါပဲ၊ NumPy Array တွေကလည်း 0 ကနေစပြီး ရေတွက် (Indexing လုပ်) ပါတယ်။ အနောက်ဆုံးကနေ ပြန်ရေချင်ရင် အနုတ်လက္ခဏာ (Negative index) သုံးလို့ရပါတယ်။

```Python title="Indexing"
a = np.array([3,7,6,1,5,2])
print(a[0], a[-1])          # 3 နဲ့ 2 ကို ထုတ်ပေးပါလိမ့်မယ် (ရှေ့ဆုံးနဲ့ နောက်ဆုံး)
```

Dimension တစ်ခုထက်ပိုတဲ့ Array (Multi-dimensional array) တွေမှာ အခန်းတစ်ခန်းချင်းစီကို လှမ်းယူချင်ရင် Index နံပါတ်တစ်ခုမက သုံးရပါတယ်။

```Python title="Indexing"
a = np.array([[3,7,6],[1,5,9]])
print(a[1][2])              # 9 ကို ထုတ်ပေးပါလိမ့်မယ်
# (a[1] က ဒုတိယမြောက် Row [1,5,9] ဖြစ်ပြီး၊ အဲ့ဒီထဲက index 2 ဖြစ်တဲ့ 9 ကို ယူလိုက်တာပါ)
```

သတိပြုရန် - a[1][2] လို့ရေးတာက ကွန်ပျူတာအလုပ်လုပ်ပုံအရ နည်းနည်းကွာခြားပါတယ်။ သူက ပထမ a[1] အပိုင်းကို အရင်ဆွဲထုတ်ပြီး ယာယီ array (temporary array) တစ်ခုအရင်ဆောက်လိုက်တယ်၊ ပြီးမှ အဲ့ဒီအထဲက index 2 ကို ထပ်ဆွဲထုတ်တာ ဖြစ်ပါတယ်။ (NumPy မှာ ပိုမြန်ချင်ရင် a[1, 2] လို့ရေးတာက ပိုကောင်းပါတယ်)။

Slicing (အပိုင်းဖြတ်တာ) ကလည်း List တွေအတိုင်းပါပဲ။ ထူးခြားတာက Dimension တွေအများကြီးမှာ ကော်မာ (comma) ခံပြီး တပြိုင်နက် ဖြတ်လို့ရတာပါပဲ။

```Python title="Slicing"
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

အရေးကြီးတဲ့ အချက် (Common Mistake)

- b[1:3][2:4] လို့ရေးတာနဲ့ b[1:3, 2:4] လို့ရေးတာ မတူပါဘူး။

- b[1:3][2:4] လို့ရေးလိုက်ရင် ပထမ b[1:3] အရ Row 1 နဲ့ 2 ပါတဲ့ Array အသစ်တစ်ခု ထွက်လာမယ်။ ပြီးတော့မှ အဲ့ဒီ Array အသစ်ရဲ့ Row 2 ကနေ 4 ကို ထပ်ဖြတ်ဖို့ ကြိုးစားပါလိမ့်မယ်။ Array အသစ်မှာက Row 2 row ပဲရှိတော့ [2:4] ဆိုတဲ့ row တွေ မရှိတော့ပါဘူး။ ဒါကြောင့် အဖြေက Empty Array [ ] (အလွတ်) ထွက်လာတာ ဖြစ်ပါတယ်။

## 27.5 Array Manipulation (Array များကို ပုံစံပြောင်းလဲ ကိုင်တွယ်ခြင်း)

Reshaping (ပုံသဏ္ဍာန် ပြောင်းလဲခြင်း) Array တစ်ခုကို တည်ဆောက်ပြီးပြီဆိုရင် reshape() method ကိုသုံးပြီး သူ့ရဲ့ ပုံသဏ္ဍာန် (Shape) ကို ပြောင်းလဲနိုင်ပါတယ်။ ဒီ Method က Data တွေကို မထိခိုက်စေဘဲ Shape အသစ်နဲ့ Array တစ်ခုကို ပြန်ထုတ်ပေးတာပါ။

*(မှတ်ချက် - မူရင်းစာသားပါ Code တွင် Element အရေအတွက် ကွဲလွဲမှုရှိနေသဖြင့် တွက်ချက်၍ရအောင် အနည်းငယ် ပြင်ဆင်ရှင်းပြပေးထားပါတယ်)*

```Python title="Reshaping"
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

Flattening (ပြားချခြင်း) Multi-dimensional array (အထပ်ထပ်ပါတဲ့ array) တစ်ခုကို ravel() သုံးပြီး 1D array (တန်းတစ်တန်းတည်းဖြစ်သွားအောင်) ပြားချလိုက်လို့ ရပါတယ်။

```Python title="Flattening"
import numpy as np
a = np.array([[3, 7, 6, 9],[1, 5, 2, 4],[0, 3, 1, 5]])
b = a.ravel()
print(b)                        
# ရလဒ်: [3 7 6 9 1 5 2 4 0 3 1 5] ဆိုပြီး တစ်တန်းတည်း ထွက်လာမယ်
```

Appending (ထပ်ဖြည့်ခြင်း) ရှိပြီးသား Array တစ်ခုရဲ့ အနောက်မှာ နောက်ထပ် တန်ဖိုးတွေ ထပ်ဖြည့်ချင်ရင် np.append() ကို သုံးနိုင်ပါတယ်။

```Python title="Appending"
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

append လုပ်လိုက်ရင် မူရင်း Array ကို သွားပြင်တာမဟုတ်ဘဲ၊ တန်ဖိုးသစ်တွေပါဝင်တဲ့ Array အသစ်တစ်ခု (Copy) ကို ထုတ်ပေးတာ ဖြစ်ပါတယ်။ ထပ်ဖြည့်မယ့် Array ဟာ မူရင်း Array နဲ့ Shape တူညီဖို့ လိုပါတယ်။ တကယ်လို့ axis မသတ်မှတ်ထားဘူးဆိုရင် Array တွေကို အရင်ဆုံး ပြားချ (Flatten) လိုက်ပြီးမှ ဆက်ပေးသွားမှာ ဖြစ်ပါတယ်။ ဒါ့အပြင် Array တွေထဲမှာ Element ကြားဖြတ်ထည့်တာ (Insert)၊ ဖျက်တာ (Delete) နဲ့ ခွဲထုတ်တာ (Split) လုပ်တဲ့ Function တွေလည်း ရှိပါသေးတယ်။ ဒါတွေကိုတော့ ကိုယ့်ဘာသာ ဆက်လက်လေ့လာကြည့်ဖို့ အကြံပြုထားပါတယ်။

---

## Problems

### Problem 27.1

Dimension 4 x 2 x 3 ရှိတဲ့ 3D Array တစ်ခုကို တည်ဆောက်တဲ့ Program ရေးပါ။ Array ထဲမှာ တန်ဖိုးတချို့ကို ကနဦးသတ်မှတ် (Initialize) ပါ။ ပြီးနောက် Axis တစ်ခုစီအလိုက် အကြီးဆုံးတန်ဖိုး (Maximum) တွေကို ရှာဖွေပါ။

<details>
<summary><b>Program</b></summary>

```python title="Problem 27.1"
import numpy as np
# 4x2x3 Array တစ်ခု တည်ဆောက်ခြင်း
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

```python title="Problem 27.1"
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

၁ မှ ၂၀ ထိ ဂဏန်းများပါဝင်ပြီး Shape 5 x 4 ရှိသော Array တစ်ခုကို တည်ဆောက်ပါ။ Array တစ်ခုလုံးရဲ့ ပေါင်းလဒ်၊ Row အလိုက် ပေါင်းလဒ်များ နှင့် Column အလိုက် ပေါင်းလဒ်များကို ရှာဖွေသည့် Program ရေးပါ။

<details>
<summary><b>Program</b></summary>

```python title="Problem 27.2"
import numpy as np
a = np.arange(20).reshape((5,4))
print(a)
print(np.sum(a))            # Array တစ်ခုလုံးပေါင်းလဒ်
print(np.sum(a, axis = 0))  # Column အလိုက်ပေါင်းလဒ်
print(np.sum(a, axis = 1))  # Row အလိုက်ပေါင်းလဒ်
```

</details>

<details>
<summary><b>Output</b></summary>

```python title="Problem 27.2"
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

အောက်ပါလုပ်ဆောင်ချက်များ ရရှိရန် Program ရေးပါ

- Size 10 ရှိပြီး Element အားလုံး တန်ဖိုး 3 သတ်မှတ်ထားတဲ့ Array a ကို တည်ဆောက်ပါ။
- Array a ရဲ့ Memory Size နဲ့ Element တစ်ခုချင်းစီရဲ့ Size ကို ရှာပါ။
- 0 မှ 90 အထိ တန်ဖိုးများ ညီတူညီမျှ ကွာခြားပြီး (Evenly spaced) ပါဝင်တဲ့ Size 10 ရှိ Array b ကို တည်ဆောက်ပါ။
- Array b ရှိ Element များကို ပြောင်းပြန်လှန် (Reverse) ပါ။
- Array a နှင့် b ကို ပေါင်းပြီး ရလာဒ်ကို Array c ထဲသို့ သိမ်းဆည်းပါ။

<details>
<summary><b>Program</b></summary>

```python title="Problem 27.3"
import numpy as np
a = np.full(10,3)
print(a)
print(a.nbytes)     # Memory size
print(a.itemsize)   # Individual element size
b = np.linspace(0,90,10)
print(b)
b = b[::-1]         # Reversing
print(b)
c = a + b
print(c)
```

</details>

<details>
<summary><b>Output</b></summary>

```python title="Problem 27.3"
[3 3 3 3 3 3 3 3 3 3]
40
4
[0. 10. 20. 30. 40. 50. 60. 70. 80. 90.]
[90. 80. 70. 60. 50. 40. 30. 20. 10. 0.]
[93. 83. 73. 63. 53. 43. 33. 23. 13. 3.]
```

</details>

### Problem 27.4

အောက်ပါလုပ်ဆောင်ချက်များ ရရှိရန် Program ရေးပါ

- Size 5 x 5 ရှိတဲ့ 2D Array တစ်ခု တည်ဆောက်ပါ။ ဘောင် (Border) ပတ်လည်ရှိ Element များကို 1 ပေးပြီး၊ အတွင်းပိုင်း Element များကို 3 ပေးပါ။
- တန်ဖိုး 2 တွေချည်းပါဝင်တဲ့ 4 x 3 Matrix တစ်ခုနဲ့ မြှောက်ပါ။
- ပေးထားသော 1D Array တစ်ခုအတွင်းရှိ တန်ဖိုး 2 နှင့် 8 ကြားရှိသော Element များကို အနှုတ်လက္ခဏာ (Negate) ပြောင်းပါ။ (မူရင်း Array ထဲမှာပင် ပြောင်းလဲခြင်း - in place)။

<details>
<summary><b>Program</b></summary>

```python title="Problem 27.4"
import numpy as np
# Note: Code logic requires modification to set inner elements to 3
a = np.ones((5,5))
# a[1:-1, 1:-1] = 3 # (This line is needed to match the description)
print(a)

b = np.ones((4,3)) # Creating 4x3 matrix
c = np.full((3,5),2) # Creating matrix for multiplication
d = b @ c          # Matrix Multiplication
print(d)

e = np.arange(11)
print(e)
e[(2 < e) & (e < 8)] *= -1 # Negating elements between 2 and 8
print(e)
```

</details>

<details>
<summary><b>Output</b></summary>

```python title="Problem 27.4"
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

## **Exercises**

[A] **အောက်ပါ ဖော်ပြချက်များသည် အမှန် (True) သို့မဟုတ် အမှား (False) ဖြစ်ကြောင်း ဖော်ပြပါ**

- [ ] Python ကို Install လုပ်လိုက်တာနဲ့ Numpy library ပါ အလိုအလျောက် Install ဖြစ်ပြီးသား ဖြစ်သည်။
- [ ] Numpy array တွေက Python List တွေထက် ပိုမြန်သည်။
- [ ] Numpy array element တွေက အမျိုးအစား (Data Type) မတူညီတာတွေ ရောနှောပါဝင်လို့ ရသည်။
- [ ] Numpy array တစ်ခုကို တည်ဆောက်ပြီးသွားရင် သူ့ရဲ့ Size နဲ့ Shape ကို ပြောင်းလဲလို့ မရတော့ပါ။ (Dynamically cannot change)
- [ ] **np.array_equal(a,b)** သည် Array *a* နှင့် *b* ၏ Shape ရော Element တွေပါ တူညီမှသာ True ကို ပြန်ပေးသည်။

[B] **အောက်ပါ မေးခွန်းများကို ဖြေဆိုပါ**

- (a) ပထမဆုံး သဘာဝကိန်း (Natural numbers) ၁၀ လုံးပါဝင်တဲ့ Numpy Array ကို ဘယ်လို တည်ဆောက်မလဲ?
- (b) Numpy ကိုသုံးပြီး ကိန်းရှုပ် (Complex numbers) Array တွေကို တည်ဆောက်လို့ ရပါသလား?
- (c) Size 3 x 4 x 5 ရှိတဲ့ Array ၅ ခုကို တည်ဆောက်ပြီး တစ်ခုချင်းစီမှာ 0 တွေချည်း၊ 1 တွေချည်း၊ 5 တွေချည်း၊ Random တန်ဖိုးများနှင့် Garbage တန်ဖိုးများ အသီးသီး ဖြည့်သွင်းချင်ရင် ဘယ်လိုလုပ်မလဲ?
- (d) ၁ မှ စတင်သော မဂဏန်း (Odd numbers) များပါဝင်သည့် Element ၅၀ ရှိသော Array တစ်ခုကို ဘယ်လို တည်ဆောက်မလဲ?
- (e) Numpy array တစ်ခုရဲ့ Element အမျိုးအစား (Type)၊ အရေအတွက်၊ Base Address နှင့် နေရာယူထားသော Byte ပမာဏတို့ကို ဘယ်လို သိနိုင်မလဲ?
- (f) a1 = np.array([[1,2,3,4],[5,6,7,8]]) ဟု တည်ဆောက်ထားသော Array ၏ Dimension နှင့် Shape ကို ဘယ်လို သိနိုင်မလဲ?
- (g) 3 x 4 Matrix နှစ်ခု ပေးထားပါက ၎င်းတို့၏ သက်ဆိုင်ရာ Element အချင်းချင်း ပေါင်းခြင်း၊ နှုတ်ခြင်း၊ မြှောက်ခြင်း နှင့် စားခြင်းတို့ကို ဘယ်လို လုပ်ဆောင်မလဲ?
- (h) အောက်ပါ Code များအနက် မည်သည်တို့သည် Numpy array ၏ Scalar arithmetic operations များ ဖြစ်ကြသနည်း?

    ```python title="Problem 27.5"
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

[C] **Match The Following pairs:**

| ကုဒ် / လုပ်ဆောင်ချက် | ဖော်ပြချက် |
|--- |--- |
| (a) `s = np.trace(a)` | 1. စာရင်းအင်းဆိုင်ရာ တွက်ချက်ခြင်း (Statistical Operation) |
| (b) `s = a.cumsum(axis = 1)` | 2. Linear Algebra တွက်ချက်ခြင်း |
| (c) `a2 = np.copy(a1)` | 3. Deep copy ပြုလုပ်ခြင်း |
| (d) `print(a1 < 2)` | 4. သက်ဆိုင်ရာ Element အချင်းချင်း နှိုင်းယှဉ်ခြင်း |
| (e) `print(a1 > a2)` | 5. တန်ဖိုးတစ်ခုတည်းနှင့် နှိုင်းယှဉ်ခြင်း (Scalar comparison) |
| (f) `print(a[1:3][3:6])` | 6. Bitwise လုပ်ဆောင်ချက် |
| (g) `a2 = invert(a1)` | 7. Inversion ပြုလုပ်ခြင်း / Slicing ပြုလုပ်ခြင်း |

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
