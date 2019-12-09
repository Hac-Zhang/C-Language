# **stirng类型**

## 简介:
> C++标准库提供的类型:string   
> 长度可变的字符串   
> 操作简单  
> &emsp;***仅为包含个人常用函数***

## 头文件

string 类型与其它的标准库类型相同，都需要包含对应的头文件

```C++
#include<string>
using namespace std;
```

## string 类型的定义和初始化

定义及初始化         | 解释
--------------------|----------------------------------------
string s1 = "C++";  | 创建字符串s1, 如果省略 *= "C++"* 则为空串
stirng s2(s1);      | 创建字符串s2并初始化值为s1的值(*C++*)
string s3("Love")   | 创建字符串s3并初始化为 *Love*
string s4(6,'I')    | 创建字符串s4并初始化为连续6个字符为'I'，组成的字符串

## string 类型的函数

* 字符串的赋值

    ```C++
    string s1 = "I LOVE C++";
    string s2;
    s2 = s1;
    cout<<s2;
    ```
    输入及输出:
    > I LOVE C++

* 字符串的 +,+= 运算符

    ```C++
    string s1 = "I ";
    string s2 = "LOVE ";
    string s3 = "C++";
    s1 = s1 + s2;
    cout<<s1<<endl;
    s1 += s3;
    cout<<s1<<endl;
    ```
    输入及输出:
    > I LOVE    
    > I LOVE C++

* 字符串的关系运算符
 
    string 类型可以直接使用==,!=,>,<,>=,<=等关系运算符来进行字符串的比较,并返回布尔类型

    ```c++
    //EG:
    string s1 = "123";
    string s2 = "123";
    cout<<(s1 == s2 ? "s1 = s2" : "s1 != s2");
    ```
    输入及输出:
    > s1 = s2

* 字符串的读取

    1. cin方式  

        读取时自动忽略开头的空白字符  
        当读取到字符后一旦遇到空白字符,结束读取  

        ```C++
        string s1;  
        cin>>s1;  
        cout<<s1;  
        ```

        输入及输出:
        
        > Hello World  
        > Hello


    2. getline方式  
    
        包含在 string 库内  

        1. `istream& getline (istream& is, string& str);`  

            ```C++
            string str;
            getline(cin,str);
            cout<<str;
            ```
            输入及输出:

            > Hello World  
            > abc  
            > Hello World

            每次输入为一行, 遇到'\n'结束输入

        2. `istream& getline (istream& is, string& str, char delim);`

            ```C++
            string str;
            getline(cin,str,'#');
            cout<<str;
            ```
            输入及输出:
            > abc def#abc  
            > abc def
            
            当以'#'为结尾术符,'#'及'#'以后的字符就不再读取

* 字符串长度  

    size()/lenth()均可, 返回该字符串的长度(字节长度)

    ```C++
    string s1;
    cout<<s1.size()<<endl;
    cout<<s1.lenth()<<endl;

    s1 = "Hello World";
    cout<<s1.size()<<endl;
    cout<<s1.lenth()<<endl;
    
    s1 = "你好";
    cout<<s1.size()<<endl;
    cout<<s1.lenth()<<endl;
    ```
    
    输入及输出:
    > 0  
    > 0  
    > 11   
    > 11  
    > 4  
    > 4  

* 字符串获取字符

    str[n]:返回str中的第n个字符,从0到size()-1

    ```C++
    string str = "I Love C++"
    cout<<str[0]<<endl;
    a[7] = 'A';
    cout<<str;
    ```

    输入及输出:
    > I  
    > I Love A++

* 字符串判空

    empty() 返回布尔类型

    ```C++
    string s1;
    if(s1.empty())
        cout<<"s1字符串为空";
    ```
    
    输入及输出:
    > s1字符串为空

* 字符串查找

    string中的find()返回值是第一次字符或字符串出现的下标,如果没找到，那么会返回npos。

    ```C++
    string s1 = "C++";
    string s2 = "I LOVE C++";
    cout<<s1.find(s2)<<endl;
    cout<<s1.find("Hello")<<endl;
    ```
    输入及输出:
    > 7  
    > 4294967295  (极大的值或极小的值)

* 字符串内的排序

    ```C++
    string str = "cba";
    sort(str.begin(), str.end());
    cout<<str;
    ```
    输入及输出:
    > abc

