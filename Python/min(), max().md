## π min()
+ μΈμλ‘ λ°μ μλ£ν λ΄μμ μ΅μκ°μ μ°Ύμμ λ°ννλ ν¨μ
+ min(x)μμ xλ __iterable__ ν μλ£ν
+ __iterable__: λ°λ³΅μ΄ κ°λ₯ν λ°μ΄ν° νμ μ¦, memberλ₯Ό νλμ© λ°ν(μ κ·Ό)ν  μ μλ λ°μ΄ν° νμ. ex) λ¦¬μ€νΈ, νν, λ¬Έμμ΄

```python
array = [4, 6, 7, 9, 2, 1]
print(min(array))
print(type(min(array)))

# 1
# <class 'int'>
```
+ λΉκ΅ λ°μ΄ν°λ€ κ° νμμ΄ κ°μμΌν¨
```python
array = ['4', 6, 7, 9, 2, 1]
print(min(array))
print(type(min(array)))

# TypeError: '<' not supported between instances of 'int' and 'str'
```
+ λλ€μ μ¬μ© κ°λ₯
```python
a = [1, 2, 3, 4, 5]
 
b = min(a, key=lambda x: x % 2)
print(b)

# 2
```

```python
str = "Hello_World"
print(min(str))
print(type(min(str)))

# H
# <class 'str'>
```

```python
str = "Hello_W2orld"
print(min(str))
print(type(min(str)))

# 2
# <class 'str'>
```

+ λ κ° μ΄μμ μΈμλ₯Ό λ°μ μ μμ
+ μΈμ κ°μ λ°μ΄ν° νμμ΄ κ°μμΌ ν¨

```python
a = [1, 2, 3] 
b = [4, 5, 6] 
print(min(a, b))
print(type(min(a, b)))

# [1, 2, 3]
# <class 'list'>
```
```python
a = 'BlockDMask' 
b = 'BAAAlockDMask' 
print(min(a, b))
print(type(min(a, b)))

# BAAAlockDMask
# <class 'str'>
```

## π max()
+ μΈμλ‘ λ°μ μλ£ν λ΄μμ μ΅λκ°μ μ°Ύμμ λ°ννλ ν¨μ
+ mix() ν¨μμ μ¬μ©λ² κ°μ

μΆμ²: https://blockdmask.tistory.com/411
