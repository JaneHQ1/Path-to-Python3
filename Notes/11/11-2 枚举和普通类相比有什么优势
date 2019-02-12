"""
11-2 枚举和普通类相比有什么优势
"""
from enum import Enum

# 如果没有枚举类，怎样表示类型？
# 用模块里的变量表示类型：
yellow = 1
green = 2

# 用字典的方式表示类型：
a = {'yellow':1, 'green':2}
a['yellow'] = 3  # 非常容易改变取值
# 最贴近于枚举

# 定义一个class：
class TypeDiamond():
    yellow = 1
    green = 2

# 以上的三种方法有两个缺陷：
# 可变，非常轻易地改变他们地值。
# 类型被确定下来以后是不应该被改变的。这也是为什么我们定义Enum子类VIP里的类型要大写。大写的意义是常量。
# 没有防止相同值得功能。
# 不同的数值用不同的类表示,以上三种数据结构允许不同标签使用相同数值.



# 在一个类里定义一个常量.
# Python并没有常量的概念,大写以后看似是常量,但实际上还是变量.
# 常量不能更改,变量是可以更改的.

class VIP(Enum):
    YELLOW = 1
    GREEN = 2
    BLACK = 3
    RED = 4

class Common():
    YELLOW = 1

# VIP.YELLOW = 6
# 报错

Common.YELLOW = 6
print(Common.YELLOW)

# 6
# 更改成功

# 枚举中两个标签相同
'''
class VIP(Enum):
    YELLOW = 1
    YELLOW = 2
    BLACK = 3
    RED = 4
'''
# 报错 Attempted to reuse key: 'YELLOW'
# 同一个标签表示两种数据是不可取的.

# Summary
# 继承Enum和不继承Enum的差别很大.
# 可变
# 没有防止相同值的功能.
# 如果表示类型最好用Enum.

