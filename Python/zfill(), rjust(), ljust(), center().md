## π zfill() λ©μλ
+ zfill(width: int)
+ λ¬Έμμ΄ μμ __0__ μΌλ‘ μ±μ°κ³  μΆμ λ μ¬μ©
+ μΈμλ μλ¦Ώμλ₯Ό μλ―Έ (integer)
+ λ°ν νμμ ```string```μ΄λ©° λ¬Έμμ΄λ‘λ§ μ¬μ© κ°λ₯ (λ€λ₯Έ νμμ λ£μΌλ©΄ μλ¬ λ°μ)
+ μλ³Έ λ¬Έμμ΄μ λ°λμ§ μμ

```python
str = 'abcd'

print(str.zfill(6))
print(type(str.zfill(6)))
print(str)

# 00abcd
# <class 'str'>
# abcd
```

## π rjust(), ljust(), center() λ©μλ
+ (width, [fillchar])
+ λ¬Έμμ΄ μμ __μνλ λ¬Έμ__ λ‘ μ±μ°κ³  μΆμ λ μ¬μ©
+ λ°ν νμμ ```string``` μ΄λ©° λ§μ°¬κ°μ§λ‘ λ¬Έμμ΄λ‘λ§ μ¬μ© κ°λ₯
+ ```rjust()```: μ€λ₯Έμͺ½ κΈ°μ€ μ λ ¬
+ ```ljust()```: μΌμͺ½ κΈ°μ€ μ λ ¬
+ ```center()```: κ°μ΄λ° μ λ ¬
+ λ λ²μ§Έ μΈμμ μλ¬΄ κ°λ λ£μ§ μμμ κ²½μ°μλ κ³΅λ°±μΌλ‘ μ²λ¦¬
+ μλ³Έ λ¬Έμμ΄μ λ°λμ§ μμ

```python
str = 'abcd'
print(str.rjust(6))
print(str.ljust(6))
print(str.center(6))

print(str.rjust(6, '0'))
print(str.ljust(6, '0'))
print(str.center(6, '0'))

print(str.rjust(6, '*'))
print(str.ljust(6, '*'))
print(str.center(6, '*'))

#   abcd
# abcd  
#  abcd 
# 00abcd
# abcd00
# 0abcd0
# **abcd
# abcd**
# *abcd*
```

### β λ λ²μ§Έ μΈμμλ νλμ λ¬Έμλ§ λ£μ΄μΌ ν¨
```python
print(str.rjust(6, '*-'))

# TypeError: The fill character must be exactly one character long
```

## β format()μ μ΄μ©ν΄ λ¬Έμμ΄ λ§κ³  μ μλ‘ μ¬μ©νκΈ°
+ κΈ°λ³Έμ μΌμͺ½ κΈ°μ€ μ λ ¬
+ λ°ν νμμ ```string```
```python
print(format(123, '4'))
print(format(123, '04'))
print(format(123, '10'))
print(format(123, '010'))

print(type(format(123, '05')))

print('{0:4d}'.format(123))
print('{0:04d}'.format(123))
print('{0:10d}'.format(123))
print('{0:010d}'.format(123))

print(type('{0:05d}'.format(123)))

#  123
# 0123
#        123
# 0000000123
# <class 'str'>
#  123
# 0123
#        123
# 0000000123
# <class 'str'>
```

μ°Έκ³ : https://codingpractices.tistory.com/39
