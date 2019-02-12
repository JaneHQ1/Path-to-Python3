"""
11-1 枚举其实是一个类
"""
from enum import En

# 现实生活中类型的概念怎么用编程来描述？

# 腾讯会员：绿钻 黄钻 红钻 黑钻
# 1 绿钻
# 2 黄钻
# 3 红钻
# 4 黑钻
# 用数字代表不同类型。我们现在经常将数字存在数据库里，每一个数字代表一种数据类型。
# 缺点：当我们读到数字的时候是无法知道它表示什么类型，因为数字本身没有描述性。所以数字表示类型的方式破坏了我们代码的可阅读性。

# 字典比较适合表示各种类型。但是字典不是最优的数据类型。

# 在很多编程语言里都有枚举表示不同的数据类型。
# 在Python2没有枚举类型，但是在Python3里增加了枚举类型。

# 如何在Python里编写枚举类型？

# 枚举在Python里的本质是一个类，所以我们定义一个class。
# 如果我们想让这个类成为一个枚举类型，需要继承Python提供的Enum类。
# 所有的枚举类都是Enum的子类。
# 在Python里一切都是类和对象。
# 用枚举的方式表示类型的可读性比直接在代码里写数字的可读性要高。
# Note: 枚举的标识名字最好用大写

class VIP(Enum):
    YELLOW = 1
    GREEN = 2
    BLACK = 3
    RED = 4

# print(VIP.YELLOW)

# VIP.YELLOW

# 打印的是VIP.YELLOW，而不是数字1。这是枚举的意义所在。
# 我们看代码的时候并不关心YELLOW具体的数值是多少，我们要的是类型。
# 枚举的意义在于它的标签，而不是它的数值。
# 可以把数值定义为任意的数据类型，只要不相同即可。

class VIP(Enum):
    YELLOW = 1
    GREEN = 1
    BLACK = 3
    RED = 4

print(VIP.YELLOW)
print(VIP.GREEN)
print(VIP.BLACK)
print(VIP.RED)

# VIP.YELLOW
# VIP.YELLOW
# VIP.BLACK
# VIP.RED

# 如果数据相同，就会显示相同的标签。

