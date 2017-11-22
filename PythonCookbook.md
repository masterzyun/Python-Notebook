# Python Cookbook Learn Notebook

# 第一章 数据结构和算法

## 问题1

*将序列分解为单独的变量*

任何序列（或可迭代的对象）都可以通过一个简单的赋值操作来分解为单独的变量。唯一的要求是变量的总数和数据结构要与序列相吻合。

```
data = ['ACME', 50, 91.1, (2012, 12, 21)]
name, shares, price, date = data
>>>name
'ACME'
>>>date
(2012, 12, 21)
```

*从任意长度的可迭代对象中分解元素*

利用"*表达式"来解决这个问题

相当于*arge

```
user_record = ('Dave', 'dave@example.com', '777-555-1212', '847-555-1212')
name, email, *phone_numbers = user_record
>>>name
'Dave'
>>>email
'dave@example.com'
>>>phone_numbers
['777-555-1212', '847-555-1212']
```

总结：将一个序列分解为各个单独的变量，可以分别赋值，也可以使用*arge表达式，可变参数的方法分解。