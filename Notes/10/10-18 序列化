"""
10-18 序列化
"""
import json

# 每一种Json数据格式都可以再Python里找到一个对应的数据类型。

# Json      Python
# object    dict
# array     list
# string    str
# number    int
# number    float
# true      True
# false     False
# null      None

# 如果你精通一门语言，那么你入门其他语言会比较容易。
# 现在大部分语言都是类C语言。

# 序列化
# 把Python数据类型像Json字符串转换的过程。

# Define a dict
student = [
    {'name':'qiyue', 'age':18, 'flag':False},
    {'name':'qiyue', 'age':18}
]
# 如果想让代码看起来舒服，尽量避免用反斜杠换行，巧妙运用括号换行。

json_str = json.dumps(student)
print(json_str)
print(type(json_str))

# [{"name": "qiyue", "age": 18, "flag": false}, {"name": "qiyue", "age": 18}]
# <class 'str'>

# 并不是说和Json相关的转换叫序列化。 Python和xml之间的转换也称作为序列化或者反序列化。
# 怎么样把对象存储到数据库？数据库是二维表，没有办法表示对象的结构。
# 可以把对象序列化成json或者xml字符串，然后将字符串存储到数据库里。当需要对象的时候把字符串从数据库里读出来，再进行反序列话的过程。
# 这是一个方法，但不可取，因为效率太低了。数据库比较适合存储比较简单的数据结构。
# 把对象拆成二维表结构，也就是把对象拆成一个个属性，然后存到数据库里去。
# 如果像存储对象，用NOSQL数据库，比如说MongoDB比较适合存储序列化的对象。
# 强烈反对将对象序列化以后存到数据库里。

# Json字符串从哪里来？
# 通常是通过序列化的过程，不一定是Python，有可能是其他语言序列化以后通过服务的方式传给我们。
# 通过服务调用Json字符串
# https://api.douban.com/v2/book/27124852

