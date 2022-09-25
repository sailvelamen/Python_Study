# Python_Study

```python
print(1+1)
2+2
```

    2
    




    4




```python
4*5
```




    20




```python
10/3
```




    3.3333333333333335




```python
10%3
```




    1



### 科学运算


```python
2**3    # 2的3次方
```




    8




```python
abs(-15.6)    # 绝对值
```




    15.6




```python
round(-15.5)    # 取整
```




    -16




```python
min(2,4,6)
```




    2




```python
max(2,4,6)
```




    6




```python
1.3e5    # 1.3*10的5次方
```




    130000.0




```python
1.5e-3 
```




    0.0015




```python
0xFF
```




    255



### 基本类型


```python
tang = 3
```




    3




```python
tang
```




    3




```python
type(tang)
```




    int




```python
tang = 1.5
tang2 = int(tang)
tang2
```




    1




```python
tang_str = '123'
type(tang_str)
```




    str




```python
int(tang_str)
```




    123




```python
float(tang_str)
```




    123.0




```python
str(132)
```




    '132'




```python
tang = True
tang
```




    True




```python
type(tang)
```




    bool




```python
3 > 5
```




    False




```python
tang = 3
1 < tang < 5
```




    True



### 字符串


```python
tang_str = 'hello'
```


```python
tang = tang_str + ' python'
tang
```




    'hello python'




```python
tang_str * 3
```




    'hellohellohello'




```python
len(tang)
```




    12




```python
len(tang*2)
```




    24




```python
tang = '1 2 3 4 5'
tang
```




    '1 2 3 4 5'




```python
tang.split()    # 默认空格切分
```




    ['1', '2', '3', '4', '5']




```python
tang = '1,2,3,4,5'
tang
```




    '1,2,3,4,5'




```python
tang = tang.split(',')
tang
```




    ['1', '2', '3', '4', '5']




```python
tang_str = ' '
tang_str.join(tang)     # 插入
```




    '1 2 3 4 5'




```python
tang = 'hello python'
tang2 = tang.replace('python','world')    # 替换
tang2
```




    'hello world'




```python
tang2 = tang2.upper()    # 全部大写
tang2
```




    'HELLO WORLD'




```python
tang2.lower()
```




    'hello world'




```python
tang = "   hello python   "
tang.strip()    # 去空格
```




    'hello python'




```python
tang = "   hello python   "
tang.lstrip()    # 去除右边空格
```




    'hello python   '




```python
tang.rstrip()    # 去除左边空格
```




    '   hello python'




```python
'{} {} {}'.format('tang','yu','di')    # 格式化输出
```




    'tang yu di'




```python
'{1} {2} {0}'.format('tang','yu','di')    # 按顺序格式化输出
```




    'yu di tang'




```python
'{tang} {yu} {di}'.format(tang = 10,yu = 5,di = 2)
```




    '10 5 2'




```python
tang = 'tang yu di:'
b = 45.6
c = 777
result = '%s %.2f %d' % (tang,b,c)
result
```




    'tang yu di: 45.60 777'



### 索引
* 从前面是0开始
* 从后面是-1开始


```python
tang = 'tang yu di'
tang[1]
```




    'a'




```python
tang[5]
```




    'y'




```python
tang[-1]
```




    'i'




```python
tang[-5]
```




    'y'




```python
tang[0:2]    # 切片左闭右开
```




    'ta'




```python
tang[5:]
```




    'yu di'




```python
tang[:6]
```




    'tang y'




```python
tang[1:-2]
```




    'ang yu '




```python
tang[-3:]
```




    ' di'




```python
tang[:]
```




    'tang yu di'




```python
tang = '123456'
tang[::2]    # 隔两个取一次
```




    '135'



### 列表


```python
tang = []
type(tang)
```




    list




```python
tang = [1,2,3,4]
tang
```




    [1, 2, 3, 4]




```python
tang = ['1','2','3']
tang
```




    ['1', '2', '3']




```python
tang = [1,'tang',3.5]
tang
```




    [1, 'tang', 3.5]




```python
tang = list([1,2,3])
type(tang)
```




    list




```python
len(tang)
```




    3




```python
a = [123,456]
b = ['ji','fan']
c = a + b     # c中的数据是拷贝的 
c
```




    [123, 456, 'ji', 'fan']




```python
a * 2
```




    [123, 456, 123, 456]




```python
c[:]
```




    [123, 456, 'ji', 'fan']




```python
a[0] = 213
a
```




    [213, 456]




```python
a[:] = ['tang','yu']
print(a)
c
```

    ['tang', 'yu']
    




    [123, 456, 'ji', 'fan']




```python
a=[1,2,3,4,5,6,7,8,9]
a
```




    [1, 2, 3, 4, 5, 6, 7, 8, 9]




```python
del a[0]
a
```




    [2, 3, 4, 5, 6, 7, 8, 9]




```python
del a[3:]
a
```




    [2, 3, 4]




```python
8 not in a    # 判断
```




    True




```python
a = [1,2,[3,4]]
a
```




    [1, 2, [3, 4]]




```python
a[2]
```




    [3, 4]




```python
a[2][1]
```




    4




```python
tang = ['apple','banana','apple','banana','apple','banana','apple','banana']
tang.count('apple')    # 计数
```




    4




```python
tang = ['apple','1','2','3','4','5','6']
print(tang.index('2'))    # 寻找下标
tang.index('apple')
```

    2
    




    0




```python
tang = []
tang.append('tang')
tang
```




    ['tang']




```python
tang.append(['yu','di'])    # 添加
tang
```




    ['tang', ['yu', 'di']]




```python
tang.insert(1,'python')
print(tang)
tang.insert(1,'tang')
```

    ['tang', 'python', 'tang', 'python', ['yu', 'di']]
    


```python
tang.remove('python')    # 从前向后删除
tang
```




    ['tang', 'tang', 'tang', 'python', ['yu', 'di']]




```python
tang.pop(4)    # 弹出
```




    ['yu', 'di']




```python
tang
```




    ['tang', 'tang', 'tang', 'python']




```python
tang = [1,3,5,2,4,6,7]
tang.sort()    # 排序
tang
```




    [1, 2, 3, 4, 5, 6, 7]




```python
tang = [1,3,5,2,4,6,7]
tang2 = sorted(tang)
tang2
```




    [1, 2, 3, 4, 5, 6, 7]




```python
tang = ['di','yu','tang']
tang.reverse()    # 反转列表
tang
```




    ['tang', 'yu', 'di']



### 字典


```python
tang = {}
type(tang)
```




    dict




```python
tang = dict()
type(tang)
```




    dict




```python
tang
```




    {}



#### 字典结构操作
key - value


```python
tang['first'] = 123
tang
```




    {'first': 123}




```python
tang['python'] = 456
tang
```




    {'first': 123, 'python': 456}




```python
tang['python']
```




    456




```python
tang['python'] = 789
tang
```




    {'first': 123, 'python': 789}




```python
tang = {'tang':123,'yu':456,'di':789}   # 字典中没有顺序
tang
```




    {'tang': 123, 'yu': 456, 'di': 789}




```python
tang_value = [1,2,3]
tang = {}
tang['yudi'] = tang_value
tang['yudi2'] = 3
tang['yudi3'] = '123'
tang
```




    {'yudi': [1, 2, 3], 'yudi2': 3, 'yudi3': '123'}




```python
tang = {}
d1 = {'tang':123,'yudi':456}
d2 = {'tang2':456,'yudi2':'789'}
tang['test1'] = d1
tang['test2'] = d2
tang
```




    {'test1': {'tang': 123, 'yudi': 456}, 'test2': {'tang2': 456, 'yudi2': '789'}}




```python
tang = dict([('tang',123),('yudi',456)])
tang
```




    {'tang': 123, 'yudi': 456}




```python
tang['tang'] += 1
tang
```




    {'tang': 124, 'yudi': 456}




```python
tang.get('tang')
```




    124




```python
tang['tang']
```




    124




```python
tang.get('fengzi','meiyou') # 如果没有对应的键可以指定输出值
```




    'meiyou'




```python
tang    # get()并不会将值放入字典中
```




    {'tang': 124, 'yudi': 456}




```python
tang.pop('tang') # 弹出元素
```




    124




```python
tang
```




    {'yudi': 456}




```python
del tang['yudi'] # 删除元素
tang
```




    {}




```python
tang = {'tang':123,'yudi':456}
tang2 = {'tang':789,'python':888}
tang.update(tang2)      # 更新操作
tang
```




    {'tang': 789, 'yudi': 456, 'python': 888}




```python
print('hello' in tang)
'tang' in tang
```

    False
    




    True




```python
print(tang.keys())
tang.values()
```

    dict_keys(['tang', 'yudi', 'python'])
    




    dict_values([789, 456, 888])




```python
tang.items()
```




    dict_items([('tang', 789), ('yudi', 456), ('python', 888)])



### 集合(set)
保存不重复的信息


```python
tang = [123,123,456,789]
tang = set(tang)
tang
```




    {123, 456, 789}




```python
tang = set()
type(tang)
```




    set




```python
tang = set([123,123,456,456,789])
tang
```




    {123, 456, 789}




```python
tang = {1,1,1,3,3,4}
tang
```




    {1, 3, 4}



#### 集合操作


```python
a = {1,2,3,4}
b = {2,3,4,5}
```


```python
a.union(b)  # 求并集
```




    {1, 2, 3, 4, 5}




```python
b.union(a)
```




    {1, 2, 3, 4, 5}




```python
a | b   # 并集
```




    {1, 2, 3, 4, 5}




```python
a.intersection(b)   # 交集
```




    {2, 3, 4}




```python
a & b   # 交集
```




    {2, 3, 4}




```python
print(a - b)
a.difference(b)
```

    {1}
    




    {1}




```python
print(b -a)
b.difference(a)
```

    {5}
    




    {5}




```python
a = {1,2,3,4,5,6}
b = {2,3,4}
```


```python
print(b.issubset(a))    # 子集
a.issubset(b)
```

    True
    




    False




```python
print(b <= a)
b > a
```

    True
    




    False




```python
a = {1,2,3}
a.add(4)
a
```




    {1, 2, 3, 4}




```python
a.update([4,5,6])
a
```




    {1, 2, 3, 4, 5, 6}




```python
a.remove(3)
a
```




    {1, 2, 4, 5, 6}




```python
a.pop()
a
```




    {2, 3, 4, 5, 6}




```python
tang = 1000
yudi = tang
print(id(tang))
id(yudi)    # 指向同一块区域
```

    2233475349136
    




    2233475349136




```python
tang is yudi
```




    True




```python
yudi = 1234
tang is yudi
```




    False




```python
tang = 1000     # 大数目值指向不同区域
yudi = 1000
print(id(tang))
id(yudi)
```

    2233475349200
    




    2233475349872




```python
tang = 1    # 小数目值指向一块区域
yudi = 1
print(id(tang))
id(yudi)
```

    2235514579248
    




    2235514579248



### 判断结构


```python
tang = 100
if tang > 50:
    print('ok')
print('test')
```

    ok
    test
    


```python
tang = 300
if tang > 200:
    print('200')
elif tang < 100:
    print('100')
else:
    print('100-200')
```

    200
    


```python
tang = [123,456,789]
if 123 in tang:
    print('ok')
```

    ok
    


```python
tang = {'tang':123,'yudi':456}
if 'yudi' in tang:
    print('ok')
```

    ok
    

### 循环结构


```python
tang = 0
while tang < 5:
    print(tang)
    tang += 1   # pyhton没有 i++ 的操作
```

    0
    1
    2
    3
    4
    


```python
tangs = {'tang','yu','di'}
# tang = set(['tang','yu','di'])
while tangs:
    tang = tangs.pop()
    print(tang)
```

    tang
    di
    yu
    


```python
tangs = set(['tang','yu','di'])
for name in tangs:
    print(name)
```

    tang
    di
    yu
    


```python
for i in range(5):  # 从0-5依次遍历
    print(i)
```

    0
    1
    2
    3
    4
    


```python
tang = [123,435,1234,513245,11243,1234]
for i in range(3):
    print(tang[i])
```

    123
    435
    1234
    


```python
for i in range(len(tang)):
    print(tang[i])
```

    123
    435
    1234
    513245
    11243
    1234
    


```python
tang = [10,11,12,13,14,15]
for i in tang:
    if i %2 == 0:
        print(i)
    else:
        # continue
        break
    print('-')
```

    10
    -
    

### 函数


```python
a = 10
b = 20
def print_value():
    print('a=',a)
    print('a=',a)
    print('a=',a)
print_value()
```

    a= 10
    a= 10
    a= 10
    


```python
def add_ab(a = 1,b = 2):    # 指定默认值
    # print(a+b)
    return (a+b)
tang = add_ab(3,5)
tang
```




    8




```python
print(add_ab())
print(add_ab(3))
add_ab(a = 0,b = 1)
```

    3
    5
    




    1




```python
def add_number(a, *args):
    b = 0
    for i in args:
        a += i
        b += a
    return a,b
a,b = add_number(1,2,3)
print(a,b)
```

    6 9
    


```python
def add_number2(a,**kwargs):    # 键值对格式
    for arg,value in kwargs.items():
        print(arg,value)
add_number2(2,x=3,y=4)
```

    x 3
    y 4
    

### 模块与包


```python
%%writefile tang.py 

tang_v = 10

def tang_add(tang_list):
    tang_sum = 0
    for i in range(len(tang_list)):
        tang_sum += tang_list[i]
    return tang_sum

tang_list = [1,2,3,4,5]
print(tang_add(tang_list))
```

    Writing tang.py
    


```python
%run tang.py
```

    15
    


```python
import tang     # 导入脚本/包
```

    15
    


```python
import tang     # 导入一次会记录
```


```python
tang
```




    <module 'tang' from 'd:\\Workspace\\JupyterNotebook\\tang.py'>




```python
print(tang.tang_v)
```

    10
    


```python
tang.tang_v = 100
tang.tang_v
```




    100




```python
print(tang.tang_list)
tang_list = [10,11,12]
tang_list
```

    [1, 2, 3, 4, 5]
    




    [10, 11, 12]




```python
tang.tang_add(tang_list)
```




    33




```python
import tang as tg

print(tg.tang_v)
tg.tang_add(tang_list)
```

    100
    




    33




```python
from tang import tang_v,tang_add

print(tang_v)
tang_add(tang_list)
```

    100
    




    33




```python
from tang import *      # 全部导入

tang_list
```




    [1, 2, 3, 4, 5]




```python
import os

os.remove('tang.py')   # 会删除tang.py文件 
```

### 异常


```python
import math

for i in range(10):
    input_number = input('write a number')
    if input_number == 'q':
        break
    result = math.log(float(input_number))
    print(result)
```


    ---------------------------------------------------------------------------

    ValueError                                Traceback (most recent call last)

    d:\Workspace\JupyterNotebook\PythonBasics.ipynb Cell 175 in <cell line: 3>()
          <a href='vscode-notebook-cell:/d%3A/Workspace/JupyterNotebook/PythonBasics.ipynb#Y341sZmlsZQ%3D%3D?line=4'>5</a> if input_number == 'q':
          <a href='vscode-notebook-cell:/d%3A/Workspace/JupyterNotebook/PythonBasics.ipynb#Y341sZmlsZQ%3D%3D?line=5'>6</a>     break
    ----> <a href='vscode-notebook-cell:/d%3A/Workspace/JupyterNotebook/PythonBasics.ipynb#Y341sZmlsZQ%3D%3D?line=6'>7</a> result = math.log(float(input_number))
          <a href='vscode-notebook-cell:/d%3A/Workspace/JupyterNotebook/PythonBasics.ipynb#Y341sZmlsZQ%3D%3D?line=7'>8</a> print(result)
    

    ValueError: math domain error



```python
import math

for i in range(5):
    try:
        input_number = input('write a number')
        if input_number == 'q':
            break
        result = math.log(float(input_number))
        print(result)
    except ValueError:
        print('ValueError: input must > 0')
        break
```

    0.0
    0.6931471805599453
    1.0986122886681098
    ValueError: input must > 0
    


```python
import math

for i in range(5):
    try:
        input_number = input('write a number')
        if input_number == 'q':
            break
        result = 1 / math.log(float(input_number))
        print(result)
    except ValueError:
        print('ValueError: input must > 0')
    except ZeroDivisionError:
        print('ZeroDivisionError: input must > 1')
```

    1.4426950408889634
    ZeroDivisionError: input must > 1
    ValueError: input must > 0
    

#### 自定义异常


```python
class TangError(ValueError):
    pass
cur_list = ['tang','yu','di']
while True:
    cur_input = input()
    if cur_input not in cur_list:
        raise TangError('Invalid input: %s' %cur_input)
```


    ---------------------------------------------------------------------------

    TangError                                 Traceback (most recent call last)

    d:\Workspace\JupyterNotebook\PythonBasics.ipynb Cell 179 in <cell line: 5>()
          <a href='vscode-notebook-cell:/d%3A/Workspace/JupyterNotebook/PythonBasics.ipynb#Y345sZmlsZQ%3D%3D?line=4'>5</a> cur_input = input()
          <a href='vscode-notebook-cell:/d%3A/Workspace/JupyterNotebook/PythonBasics.ipynb#Y345sZmlsZQ%3D%3D?line=5'>6</a> if cur_input not in cur_list:
    ----> <a href='vscode-notebook-cell:/d%3A/Workspace/JupyterNotebook/PythonBasics.ipynb#Y345sZmlsZQ%3D%3D?line=6'>7</a>     raise TangError('Invalid input: %s' %cur_input)
    

    TangError: Invalid input: tang2



```python
try:
    1 / 0
except:
    print('==0')
finally:
    print('finally')
```

    ==0
    finally
    

### 文件操作


```python
%%writefile tang.txt
hello python_branch
tang yu di
jin tian tian qi bu cuo
```

    Writing tang.txt
    

#### 读


```python
txt = open('./tang.txt')
txt_read = txt.read()
print(txt_read)
```

    hello python_branch
    tang yu di
    jin tian tian qi bu cuo
    
    


```python
txt = open('./tang.txt')
lines = txt.readlines()
print(type(lines))
lines
```

    <class 'list'>
    




    ['hello python_branch\n', 'tang yu di\n', 'jin tian tian qi bu cuo\n']




```python
for line in lines:
    print(line)
```

    hello python_branch
    
    tang yu di
    
    jin tian tian qi bu cuo
    
    


```python
txt.close()
```

#### 写


```python
txt = open('./data/tang_write.txt','w')
txt.write('jin tian tian qi bu cuo\n')
txt.write('tang yu di')
txt.close()
```


```python
# 'w' 操作会覆盖
txt = open('./data/tang_write.txt','w')
txt.write('1234\n')
txt.write('456\n')
txt.close()
```


```python
txt = open('./data/tang_write.txt','a')
txt.write('tangyudi\n')
txt.write('790982635')
txt.close()
```


```python
txt = open('./data/tang_write.txt','w')
for i in range(5):
    txt.write(str(i) + '\n')
txt.close()
txt2 = open('./data/tang_write.txt','r')
print(txt2.read())
```

    0
    1
    2
    3
    4
    
    


```python
txt = open('./data/tang_write.txt','w')
try:
    for i in range(100):
        txt.write(str(i) + ' '  + str(10 / (i -50)) + '\n')
except Exception:
    print('error:',i)
finally:
    txt.close()
```

    error: 50
    


```python
# 'with' 方法可以自动关闭
with open('./data/tang_write.txt','w') as f:
    f.write('jin tian tian qi bu cuo\n')
```

### 类：面向对象


```python
class people:
    'help:xxxx'
    number = 100

    def __init__(self,name,age):    # 相当于构造函数
        self.name = name
        self.age = age
    def display(self):
        print('number = :',self.number)
    def display_name(self):
        print(self.name)
```


```python
people.__doc__
```




    'help:xxxx'




```python
p1 = people('tang',30)
p2 = people('python',40)
```


```python
print(p1.name)
p2.name
```

    tang
    




    'python'




```python
print(p1.display())
p2.display()
```

    number = : 100
    None
    number = : 100
    


```python
p2.name = 'hello'
p2.name
```




    'hello'




```python
del p2.name # 删除属性
p2.name
```


    ---------------------------------------------------------------------------

    AttributeError                            Traceback (most recent call last)

    d:\Workspace\JupyterNotebook\PythonBasics.ipynb Cell 202 in <cell line: 1>()
    ----> <a href='vscode-notebook-cell:/d%3A/Workspace/JupyterNotebook/PythonBasics.ipynb#Y406sZmlsZQ%3D%3D?line=0'>1</a> del p2.name # 删除属性
          <a href='vscode-notebook-cell:/d%3A/Workspace/JupyterNotebook/PythonBasics.ipynb#Y406sZmlsZQ%3D%3D?line=1'>2</a> p2.name
    

    AttributeError: name



```python
hasattr(p1,'name') # 判断属性是否存在
```




    True




```python
hasattr(p1,'sex')
```




    False




```python
setattr(p1,'name','yudiTang')   # 内置get/set方法
getattr(p1,'name')  
```




    'yudiTang'




```python
delattr(p1,'name')  # 删除属性
p1.name
```


    ---------------------------------------------------------------------------

    AttributeError                            Traceback (most recent call last)

    d:\Workspace\JupyterNotebook\PythonBasics.ipynb Cell 206 in <cell line: 2>()
          <a href='vscode-notebook-cell:/d%3A/Workspace/JupyterNotebook/PythonBasics.ipynb#Y413sZmlsZQ%3D%3D?line=0'>1</a> delattr(p1,'name')
    ----> <a href='vscode-notebook-cell:/d%3A/Workspace/JupyterNotebook/PythonBasics.ipynb#Y413sZmlsZQ%3D%3D?line=1'>2</a> p1.name
    

    AttributeError: 'people' object has no attribute 'name'



```python
print(people.__doc__)
print(people.__name__)    # 类的名字
print(people.__module__)  # 类的模块
print(people.__bases__)   # 父类
print(people.__dict__)    # 类的组成
```

    help:xxxx
    people
    __main__
    (<class 'object'>,)
    {'__module__': '__main__', '__doc__': 'help:xxxx', 'number': 100, '__init__': <function people.__init__ at 0x0000024024B5B4C0>, 'display': <function people.display at 0x0000024024B5B790>, 'display_name': <function people.display_name at 0x0000024024B5B5E0>, '__dict__': <attribute '__dict__' of 'people' objects>, '__weakref__': <attribute '__weakref__' of 'people' objects>}
    


```python
class Parent:   # 父类
    number = 100
    def __init__(self):
        print('父类构造函数')
    def parentM(self):
        print('调用父类方法')
    def setAttr(self,attr):
        Parent.parentAttr = attr
    def getAttr(self):
        print('父类属性：',Parent.parentAttr)
    def newM(self):
        print('父类被重写的方法')

class child(Parent):    #定义子类
    def __init__(self):
        print('调用子类构造函数')
    def childM(self):
        print('调用子类方法')
    def newM(self):
        print('子类重写')
```


```python
c = child()
c.childM()
c.parentM()
c.setAttr(100)
c.getAttr()
c.newM()
```

    调用子类构造函数
    调用子类方法
    调用父类方法
    父类属性： 100
    子类重写
    

### 时间操作


```python
import time
```


```python
time.time() # 时间戳 1970.1.1 ~ now
```




    1664123825.9112656




```python
time.localtime(time.time())
```




    time.struct_time(tm_year=2022, tm_mon=9, tm_mday=26, tm_hour=0, tm_min=38, tm_sec=27, tm_wday=0, tm_yday=269, tm_isdst=0)




```python
print(time.asctime(time.localtime(time.time())))   # 格式化输出
print(time.strftime('%Y-%m-%d %H:%M:%S',time.localtime()))
```

    Mon Sep 26 00:42:28 2022
    2022-09-26 00:42:28
    


```python
import calendar # 日历模块
print(calendar.month(2017,11))
```

       November 2017
    Mo Tu We Th Fr Sa Su
           1  2  3  4  5
     6  7  8  9 10 11 12
    13 14 15 16 17 18 19
    20 21 22 23 24 25 26
    27 28 29 30
    
    


```python
help(calendar.month)    #help()函数
```

    Help on method formatmonth in module calendar:
    
    formatmonth(theyear, themonth, w=0, l=0) method of calendar.TextCalendar instance
        Return a month's calendar string (multi-line).
    
    
