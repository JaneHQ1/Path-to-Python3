"""
11-4 枚举的比较运算
"""
from enum import Enum

# 两个枚举之间是可以进行等值比较.

class VIP(Enum):
    YELLOW = 1
    GREEN = 2
    BLACK = 3
    RED = 4

result = VIP.GREEN == VIP.BLACK
print(result)

# False

result = VIP.GREEN == VIP.GREEN
print(result)

# True

result = VIP.GREEN == 2
print(result)

# False

# 不会报错,但是不能得到正确的结果.

# 两个枚举类型是否可以进行大小比较?

# result = VIP.GREEN > VIP.BLACK
# prin(result)

# 报错,枚举类型之间不能做大小的比较.

result = VIP.GREEN is VIP.GREEN
print(result)

# True

# 枚举类型之间可以做身份比较.

# 如果是两个枚举类,是否可以做等值比较?

class VIP1(Enum):
    YELLOW = 1
    GREEN = 2
    BLACK = 3
    RED = 4

result = VIP.GREEN == VIP1.GREEN
print(result)

# False

# 不会报错,但是得到False.为什么?
# 因为VIP和VIP1是两个不同的类,虽然数值相同,但根本不是同一个枚举.

# Summary
# 枚举可以做等值比较.
# 枚举可以做身份比较.
# 枚举不可以做大小比较.
# 两个不同枚举类不能作比较.

