"""
10-17 反序列化
"""
import json

# Json 的载体是str
# 我们拿到的Json可能不是字符串，而是对象。这个是有些框架默认将Json直接转换成了对象，但是我们原生拿到的就是一串字符串。

# json_str = "{name:qiyue, age:18}" 不符合 Json 字符串规范
# 'qiyue' 要加引号，表示它是字符串。
# Json字符串中的 key: name & age 也需要加引号。
# 数字类型不需要加引号。
# Python 可以用单引号表示string，但是Json是一个和语言无关的格式，规定必须使用双引号。
# 里面使用双引号，外边就用单引号。

json_str = '{"name":"qiyue", "age":18}'

# 我们要快速访问 Json 字符串中的相关信息。
# 如何拿到学生的name and age？

# 方法一：
# 就把它当作字符串，用正则表达式或者 Python 内置字符串操作获取name and age。
# 这个方法很不可取，对于复杂的数据结构，它的Json字符串会很长很复杂。

# 方法二：
# 我们每次在Python中操作数据的时候，都是用已知的数据类型()[]做一系列操作，如果用Python内置的数据结构，会比直接草做字符串要方便简单很多。
# 每一个Json字符串几乎都可以在语言里找到一个对应的数据结构，如果我们可以把和语言无关的字符串转换成字典，然后用字典访问所对应的属性，会方便很多。
# 如何用 Python 内置的 Json 操作方法把 Json 转换成已知的 Python 的数据结构？
# Python 有一个 Json 模块。 json.loads()可以帮我们把 json 字符串转换成对应的 Python 数据结构。

student = json.loads(json_str)  # 通过load函数将Json字符串转成字典
print(student)
print(type(student))
print(student['name'])
print(student['age'])

# {'name': 'qiyue', 'age': 18}
# <class 'dict'>
# qiyue
# 18

# Python 中字典的格式刚刚好和Json定义的格式相似。这里是字典，不是字符串。
# Json 字符串就是 Javascript 中的对象的格式。换言之，这串字符串在Javascript是对象，但是在Python中是字典。
# 不同语言将Json字符串转换成不同类型。Python 将 Json 字符串转成字典，但是其他语言会转换成其他格式。
# json 字符串在 Json 的数据结构里对应的是 Json 的 object，在 Python 中用字典的方式来承载object的信息。
# 在Json数据格式里，不仅仅只有 object 对象这一种数据类型，还有 array。
# 如果 Json 是一个数组，Json 字符串该怎么表示？

json_array = '[{"name":"qiyue", "age":18}, {"name":"qiyue", "age":18}]'  # 有两个 object 的 array

# 数组就是一个集合。
# 数组在 Python 里会转换成什么？

student = json.loads(json_array)  # 通过load函数将Json字符串转成字典
print(student)
print(type(student))

# [{'name': 'qiyue', 'age': 18}, {'name': 'qiyue', 'age': 18}]
# <class 'list'>

# 现在的student是一个列表，这个列表有两个字典。
# 为什么在列表中的元素是字典呢？
# 因为Json字符串的数组的内部是一个对象，Python 用字典对应对象。

json_array = '[{"name":"qiyue", "age":18, "flag":false}, {"name":"qiyue", "age":18}]'
student = json.loads(json_array)  # 通过load函数将Json字符串转成字典
print(student)
print(type(student))

# [{'name': 'qiyue', 'age': 18, 'flag': False}, {'name': 'qiyue', 'age': 18}]
# <class 'list'>

# Json 的bool是小写，Python 的 bool 是大写。

# Summary
# Json 有自己的数据类型。
# load 函数主要作用是将Json数据类型转换成Python自己的数据类型。
# 反序列话：由字符串到一个语言的数据结构。

