# Chapter 1 Introduction To Python

<div class="chapter-social-card">
  <div class="chapter-info">
    <div class="chapter-number">CHAPTER 2</div>
    <h1 class="chapter-title">Getting Started</h1>
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

### 1.1 Python Specification

* **Python** is a **specification** for a language that can be **implemented** in different ways. There are many **implementations** of this **specification** written in different languages.

* Different popular **Python implementations** are:
  * **CPython** - is the reference **implementation**, written in **C**.
  * **PyPy** - Written in a subset of **Python language** called **RPython**.
  * **Jython** - Written in **Java**.
  * **IronPython** - Written in **C#**.

* All the **implementations** are **compilers** as well as **interpreters**. The **compiler** converts the **Python program** into intermediate **bytecode**. This **bytecode** is then interpreted by the **interpreter**.

---

### 1.2 Python Installation under Windows

* **Python** has evolved over the years. At the time of writing of this edition the latest version for **Windows** and **Linux** environments was **Python 3.14.1**.

* **Python** is not shipped as part of **Windows OS**. So we need to install it separately. For this we need to download the **Python installer** from [www.python.org/downloads/](http://www.python.org/downloads/).

* While downloading ensure that you choose the appropriate **installer** from the following, based on whether you wish to install it on a **32-bit machine** or a **64-bit machine**:
  * **64-bit machine**: Download **Windows x86-64 executable installer**
  * **32-bit machine**: Download **Windows x86 executable installer**

* Once you have chosen and downloaded an **installer**, execute it by double-clicking on the downloaded file. A dialog shown in *Figure 2.1* will appear on the screen. ![Fig 2.1 Python 3.14.1 Installer Screen](../assests/fig%2021.png)

* In this dialog check the check box '**Add Python 3.14 to PATH**' or '**Add python.exe to PATH**' to ensure that the **interpreter** will be placed in your **execution path**.

* Click on '**Install Now**' and the **installation** will happen in a few minutes. **Python files** will get installed in the **directory**: `C:\Users\Joseph\AppData\Local\Programs\Python\Python314`

* In this **path** ‘**Joseph**’ represents the **user name** and ‘**Python314**’ represents the **version number** of **Python installation** that you have downloaded and installed.

* If you forget to check the **check box**, you can add the **path** mentioned above to **PATH variable** through **Control Panel** > **System** > **Environment Variables** > **Edit**. The **PATH variable** already contains many **semicolon separated values**. Append the above **path** to existing values.

* Once the **installation** is complete, you can verify it by opening a **command prompt** and typing **python --version**.

* If the **installation** was successful, you will see the version of **Python** installed on your system.

* If you are using **Windows 10**, you can also verify the **installation** by opening **Settings** > **Apps** > **Apps & features** > **Python**.

* If you are using **Windows 11**, you can also verify the **installation** by opening **Settings** > **Apps** > **Apps & features** > **Python**.

---

### 1.3 Python Installation under Linux

* Most **Linux distributions** (like **Ubuntu**) already contain **Python** in them. However, the installed **Python version** may not be the latest one. You can check the **version** as shown below:

    ```bash title="Checking Python version"
    python3 --version
    ```

* If you find that the **version** is not the latest one, then you can install the latest specific version (e.g., **Python 3.13**) using the **command**:

    ```bash title="Installing Python 3.13"
    sudo apt update
    sudo apt install python3.13
    ```

---

### 1.4 Python Resources

* **Python source code**, **binaries** and **documentation** is available at:
  * **Python official website**: [www.python.org](http://www.python.org)
  * **Documentation website**: [www.python.org/doc](http://www.python.org/doc)

* **Program development** in **Python** can be done in 3 ways:
  * Using built-in **IDLE**.
  * Using **third-party IDEs**.
  * Using **online Python shells**.

* **Third-party development tools** and the links from where they can be downloaded are given below:
  * **NetBeans IDE for Python**: [https://netbeans.apache.org/front/main/download/](https://netbeans.apache.org/front/main/download/)
  * **PyCharm IDE for Python**: [https://www.jetbrains.com/pycharm](https://www.jetbrains.com/pycharm)
  * **Visual Studio Code IDE**: [https://code.visualstudio.com/download](https://code.visualstudio.com/download)

* If you do not wish to install any **Python development tool** on your machine, then you can use any of the following **online Python shells**:

* [https://www.python.org/shell/](https://www.python.org/shell/)
* [https://ideone.com/](https://ideone.com/)
* [https://replit.com/languages/python3](https://replit.com/languages/python3)

---

### 1.5 Third-party Packages

* **Pythonistas** in **Python community** create **packages** (**libraries**) and makes it available for use for other **programmers**. They use **PyPI**—**Python Package Index** ([www.pypi.org](http://www.pypi.org)) to distribute their **packages**.

* **PyPI** maintains the list of such **third-party Python packages** available.

* There are **third-party packages** available for literally doing everything under the sun. Some **packages** that are popularly used for creating **Data Science applications** include:
  * **NumPy**: Advanced **mathematical operations library** with support for large **multi-dimensional arrays** and **matrices**.
  * **SciPy**: **Scientific computing library** for **optimization**, **integration**, **interpolation**, **signal processing**, **image processing**, etc.
  * **Pandas**: **Library** for manipulating **numerical tables** and **time series**.
  * **MatPlotLib**: **2D** and **3D Data visualization library**.
  * **OpenCV**: **Open source Computer vision library**.

### 1.6 Python Packages and Development Tools

* You too can register at **PyPI** and upload your **packages** there. You should follow the guidelines given at [www.pypi.org](http://www.pypi.org) to create the **package**, build it and upload it to the **Python Package Index**.

* **pip** is a commonly used **tool** for installing **packages** from **PyPI**. This **tool** gets installed when you install **Python**.

#### 1.6.1 Data Science and AI Tools

* Many tools have come into existence to help **Python programmers** build and document their **Data Science** and **Artificial Intelligence applications**. These include:
  * **Jupyter Notebook** - It is a very flexible **browser-based tool** that lets us to interactively work with **Python** (and many other languages). It lets us put our **Python code**, **output** of the **code** and any kind of **visualization** or **plot** etc. in the same document called **Notebook**. It is a great **tool** doing **modular program development**.
  * **Google Colab** - This **tool** provides a free **Jupyter notebook environment** to execute **code** on **Google's cloud servers**. As a result, you can leverage the power of **Google's hardware**.
  * **Spyder** - This **tool** provides a **Scientific Python Development Environment** with sophisticated **testing** and **debugging features**.

* Both **Jupyter** and **Spyder** are part of a very popular **software distribution** called **Anaconda**. So once you download and install **Anaconda**, you get **Jupyter** and **Spyder** ready-made.

#### 1.6.2 IDLE (Integrated Development and Learning Environment)

* Once **Python** is installed, **program development** can be done using the built-in **Python Integrated Development and Learning Environment** (**IDLE**).

* **IDLE** is a good **development tool**. It offers handy features like **syntax highlighting**, **context-sensitive help** and **debugging**.
  * **Syntax highlighting** feature display **keywords**, **functions**, **methods** and **strings** in different colors making it easy to identify them.
  * **Context-sensitive help** can be obtained by pressing **Ctrl Space** wherever you need help as you type the **program**. This is immensely useful since it is almost impossible to remember names of all **functions** and **methods** and their **parameters**.
  * **Debugger** lets you locate any **logical errors** that you may have committed in your **program** by allowing you trace the **flow of execution** of the **program**. This **tracing** can be done a step at a time by setting up **break points** and by **single stepping** through the **program**. As you do so **IDLE** lets you watch the **values** of different **variables** as they change during **execution**.

#### 1.6.3 Python Modes

* **Python** can be used in two **modes**:
  * **Interactive mode** - used for exploring **Python syntax**, seek help and **debug** short **programs**.
  * **Script mode** - used for writing full-fledged **Python programs**.

* Both **modes** are supported by **IDLE**.

##### **1.6.3.1 To use IDLE in Interactive mode:**

* Locate it in **Windows** by typing **IDLE** in **Windows search bar** and hit enter, or double click the **IDLE icon**.
* It will open the **Python shell window** showing `>>>` **Python shell prompt**.
* Execute the following **Python code** at this **prompt**.

    ```python title="Interactive mode"
    >>> print('Keep calm and bubble on')
    ```

* It will display the message 'Keep calm and bubble on' followed by the `>>>` **prompt**.

##### **1.6.3.2 To use IDLE in Script mode:**

* Launch **IDLE**. In the **IDLE shell window** from the **menu** select **File** | **New File**. A new window will open. Type the following **script** in it:

    ```python title="Script mode"
    print('Those who can\'t laugh at themselves…')
    print('leave the job to others.')
    ```

* Using **File** > **Save** and save the **script** under the name '**Test.py**'.
* Execute the **script** from the **Run menu** or using **F5**. The two messages will get printed.

##### **1.6.3.3 Using Other IDEs**

* Instead of **IDLE** if you decide to use **NetBeans** or **Visual Studio Code** for **program development** then follow the steps given below:
  * Create a new **Python project** ‘**Test**’.
  * Type the **script** in **Test.py**.
  * Execute the **script** using **F6** in **NetBeans** or **Ctrl F5** in **Visual Studio Code**.
  * On **execution** it will print the two lines and then you are ready to create another **project** and another **script** in it.

### 1.7 Checking Python Version

* **Python** has evolved over the years. You can determine the **version** installed on your machine through a simple **Python script**:

    ```python title="Checking Python version"
    import sys
    print(sys.version)
    ```

---

### **Exercises**

**[A] Answer the following quesitons:**

* a. What do the prompt C:\>,$ and >>> signify?
* b. In which two modes can IDLE be used?
* c. What is the purpose of the two programming modes offered by IDLE?
* d. How can third party libraries be used in a **Python Program**?

**[B] Match the following pairs:**

|Section A | Section B|
|---|---|
|a. `pip`|1. Advanced mathematical operations|
|b. `Jupyter` | 2. Scientific Computing|
|c. `Sypder` | 3. Manipulation numerical tables|
|d. `PyPI` | 4. Visualization|
|e. `Numpy`|5. Computer Vision|
|f. `Scipy` | 6. Package installation tool|
|g. `Pandas` | 7. Build and document applications|
|h. `MatPlotlib` | 8. Scientific Library|
|i. `OpenCV` | 9. Python Package index|

**[C] State whether the following statements are True or False:**

* a. Python is a specification that can be implemented through languages like **Python**,**C#**,**Java**,etc.
* b. **CPython** is implementation of **Python** specification, written in **C**.
* c. Python program is first compiled intor **byte code**, which is then interpreted.
* d. Most **Linux** distributions already contain **Python**.
* e. Windows system doesn't contain Python and it needs to be separately installed.
* f. PYthon prgorams can be built using **IDLE**, **Netbeans**, **PyCharm** and **Visual Studio Code**.
* g. Thrid-party Python packages are distributed using **PyPI**.

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
