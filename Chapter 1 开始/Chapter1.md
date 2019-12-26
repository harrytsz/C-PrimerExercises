# Chapter 1 Start

**Exercise 1.1：** 查阅你使用的编译器的文档，确定它所使用的命名约定。编译并运行第2页的 main 程序。

```c++
int main(){
    return 0;
}
```
**Exercise 1.2:** 改写程序，让它返回-1.返回值 -1 通常被当作程序错误的标识。重新编译并运行你的程序，观察你的系统该如何处理 main 返回的错误标识。

**Answer:** Win7 操作系统并不处理或报告程序返回的错误标识，直观上，返回 -1 的程序与返回 0 的程序在执行效果上并无不同。但环境变量 ERRORLEVEL 
记录了上一个程序的返回值、因此，在控制窗口执行修改后的程序，接着执行 echo %ERRORLEVEL%，会输出 -1.在 Linux 系统中，执行 echo $? 有类似的效果。

**Exercise 1.3:** 编写程序，在标准输出上打印 Hello, World。

```c++
#include<iostream>
using namespace std;
int main(){
    cout << "Hello, World" << endl;
    return 0;
}
```

**Exercise 1.4:** 我们的程序使用加法运算符+来将两个数相加。编写程序使用乘法运算符*，来打印两个数的积。

```c++
#include<iostream>
using namespace std;
int main(){
    cout << "Please input tow integers !" << endl;
    int a, b;
    cin >> a >> b;
    cout << "a * b = " << a * b << endl;
    return 0;
}
```