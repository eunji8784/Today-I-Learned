## π append()
+ array.append(x)μ ννλ‘ μ¬μ©
+ μλ‘μ΄ μμλ₯Ό array λ§¨ μ€λ₯Έμͺ½ λμ κ°μ²΄λ‘ μΆκ°
+ μλ ₯ν κ°μ΄ λ¦¬μ€νΈμ κ°μ iterable μλ£νμ΄λλΌλ κ°μ²΄λ‘ μ μ₯

```python
nums = [1, 2, 3]
nums.append(4)
print(nums)

nums.append('4')
print(nums)

nums.append([5, 6])
print(nums)

nums.append((5, 6))
print(nums)

# [1, 2, 3, 4]
# [1, 2, 3, 4, '4']
# [1, 2, 3, 4, '4', [5, 6]]
# [1, 2, 3, 4, '4', [5, 6], (5, 6)]
```

## π extend()
+ array.extend(iterable) ννλ‘ μ¬μ©
+ μλ ₯ν iterable μλ£νμ ν­λͺ© κ°κ°μ arrayμ λμ νλμ© μΆκ°
+ __μΈμλ‘ iterable μλ£νλ§ μ¬ μ μμ__ (interable μΈμκ° μλ κ²½μ° TypeError λ°μ)
+ λ³΄ν΅ interable μΈμλ₯Ό νλμ© κΊΌλ΄μ λ°°μ΄μ λ£κ³  μΆμ λ extendλ₯Ό μ¬μ©

```python
nums = [1, 2, 3]
nums.extend([4])
print(nums)

nums.extend(['4'])
print(nums)

nums.extend([5, 6])
print(nums)

nums.extend((7, 8))
print(nums)

# [1, 2, 3, 4]
# [1, 2, 3, 4, '4']
# [1, 2, 3, 4, '4', 5, 6]
# [1, 2, 3, 4, '4', 5, 6, 7, 8]
```

```python
nums = [1, 2, 3]
nums.extend(4)
print(nums)

# TypeError: 'int' object is not iterable
```

## π insert()
+ array.insert(i, x) ννλ‘ μ¬μ©
+ arrayμ μνλ μμΉ i μμ μΆκ°ν  κ° xλ₯Ό μ½μ
+ iμ μμλ₯Ό μλ ₯νλ©΄ λ°°μ΄μ μ€λ₯Έμͺ½ λμ κΈ°μ€μΌλ‘ μ²λ¦¬
+ μΆκ°ν  κ° xλ κ°μ²΄λ‘ μΆκ°λλ©° iterable μλ£νμ΄λλΌλ κ°μ²΄λ‘ μ μ₯

```python
nums = [1, 2, 3]
nums.insert(0, 4)
print(nums)

nums.insert(-1, '4') # λμμ 1λ²μ§Έ μ μ μΆκ°
print(nums)

nums.insert(len(nums), [5, 6])
print(nums)

nums.insert(len(nums), (7, 8))
print(nums)

# [4, 1, 2, 3]
# [4, 1, 2, '4', 3]
# [4, 1, 2, '4', 3, [5, 6]]
# [4, 1, 2, '4', 3, [5, 6], (7, 8)]
```
