# Python学习

## Day1

### 各种基础语句

###### Python特有虚数

```python
#虚数
x=3+5j
#输出会自动换行
print(x.real)#实部
print(x.imag)#虚部
print(type(x.real))#查询数据类型
#均为float
```

###### 字符串操作

```Python
#字符串操作——基础
a='Aa'
b="11:30 UESTC There\'s no electricity"#字符串内想写出\'"需使用\
print(a+'C\
c')#字符串合并#骚操作换行
print(a*3)#字符串叠加
#转义符\用法
print(a+'\b')#仅回退
print(a+'\b'+a)#回退后开始替换
print('%%%%%%'+'\n'+'%%%%%%%%')#进行一个行的换
print(b+'\r'+a)#将输入器移至开头
print('\t'+a)#打一个Tab
```

教材就搁着写个“退格”，“回车”，“制表”。又不给例子，指望谁看懂呢

```python
#字符串操作——高阶
a='aAa'
b="11:30 UESTC There\'s no electricity"#字符串内\'"需使用\
print(len(a))#字符串长度，同时可用于列表，集合等
print(str.upper(a))#小写转化成大写
print(str.lower(a))#大写转化成小写
print(str.capitalize(a))#首字母大写
print(a.count('a'))#搜索子字符串出现次数
print(a.strip('a'))#删除首尾字符
print(a.lstrip('a'))#left strip
print(a.rstrip('a'))#right strip
print(b.replace('E',""))#对特定子串进行替换
```

###### 特殊的基础运算符

```python
a**b#a的b次幂
a//b#整除b
#Python支持运算符使用+=，不支持++
```

```Python
#常用函数
print(abs(-1))#绝对值
print(chr(65))#返回该Unicode编码的字符
print(eval('1+1'))#执行字符串的表达式
print(int('65',8))#强制转换数据类型，int可加参表示多少进制下，但仅限于字符串，其他有float，str
print(input())#输入
print(pow(2,3,3))#a的b次幂对c取模，第三个参可省
print(round(3.1415926,3))#保留小数前几位
```

###### 基础控制结构

```python
#判断与循环
#标准输出
print(1,2,sep=' ',end='\n')
print("%d %d\n"%(1,2),end='')
#标准输入
a,b=input().split(' ')#split中为间隔符
#bool型相关
print(bool(12&0))#整数可直接当bool型使用
#python支持与c相同的位运算
#if格式
if 1 and 0:
    print(2)
elif 0:
    print(1)
else:
    print(0)
#while格式
while 0:
    print(1)
else:
    print(0)
#for格式
for i in range(1,3+1):
    print(i)
#break 与 continue存在，与C相同
```

```python
ans=0
n,m=input().split(' ')
n=int(n)
m=int(m)
b=[]
for i in range(0,n):
    b.append(1000)
for i in range(0,m):
    c = list(map(int,input().split()))
    for j in range(0,n):
        if(b[j]>c[j] and c[j]!=-1):
            b[j]=c[j]
for i in range(0,n):
    ans+=b[i]
print(ans)
```

+

