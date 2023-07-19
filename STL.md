# STL

## 容器

### string

#### string构造函数

```c++
string();		//创建一个空字符串
string(const char *s);		//使用字符串s初始化
string(const string &str);		//使用string对象初始化
string(int n, char c);		//使用n个字符c初始化
```



#### string赋值操作

```c++
string& operator=(const char *s);
string& operator=(const string &s);
string& operator=(char c);
string& assign(const char *s);
string& assign(const char*s, int n);		//赋值为字符串s前n个字符
string& assign(const string &s);
string& assign(int n, char c);		//赋值为n个字符c
```



#### string容器操作

##### 拼接

```c++
string& operator+=(const char *str);		//+=重载
string& operator+=(const char c);		//+=重载
string& operator+=(const string &str);		//+=重载
string& append(const char *s);
string& append(const char *s, int n);		//将字符串s前n个字符拼接到字符串结尾
string& append(const string &s);
string& append(const string &s, int pos, int n);		//将string对象s从pos开始n个字符拼接到字符串结尾
```

##### 查找

```c++
int find(const string &str, int pos=0) const;		//查找str第一次出现位置，从pos查找
int find(const char *s, int pos=0) const;
int find(const char *s, int pos, int n) const;		//查找s前n个字符第一次出现位置，从pos查找
int find(const char c, int pos=0) const;
int rfind(const string &str, int pos=npos) const;		//查找str最后一次出现位置，从pos查找
int rfind(const char *s, int pos=npos) const;
int rfind(const char *s, int pos, int n) const;
int rfind(const char c, int pos=0) const;
```

##### 替换

```c++
string& replace(int pos, int n, const string& str);		//替换pos开始n个字符为字符串str
string& replace(int pos, int n, const char *s);
```

##### 比较

```c++
int compare(const string &s) const;		//=返回0，>返回1，<返回-1
int compare(const char *s) const;
```

##### 存取

```c++
char& operator[](int n);		//[]重载
char& at(int n);		//通过at()方法
```

##### 插入

```c++
string& insert(int pos, const char *s);
string& insert(int pos, const string &str);
string& insert(int pos, int n, char c);		//在指定位置pos插入n个字符c
```

##### 删除

```c++
string& erase(int pos, int n=npos);		//删除从pos开始n个字符
```

##### 子串

```c++
string substr(int pos=0, int n=npos) const;		//返回pos开始n个字符组成的字符串
```



### vector

#### vector构造函数

```c++

```



#### vector赋值操作

```c++

```



#### vector容器操作

##### 容量和大小

```c++

```

##### 插入

```c++

```

##### 删除

```c++

```

##### 存取

```c++

```

##### 互换

```c++

```

##### 预留

```c++

```
