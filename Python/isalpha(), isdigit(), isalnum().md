## ๐ isalpha()
+ ๋ฌธ์์ด์ ๊ตฌ์ฑ์ด ๋ชจ๋ ์ํ๋ฒณ์ธ์ง ํ์ธํ๋ ํจ์
+ ๋ฌธ์์ด์ ์ซ์ ๋ฐ ๊ณต๋ฐฑ, ํน์๋ฌธ์๊ฐ ํฌํจ๋์ด ์์ผ๋ฉด False๋ฅผ ๋ฐํ
+ ํ๊ธ ์ง์
```python
ex1 = 'A'
ex2 = 'ABC'
ex3 = '์๋'
ex4 = 'Hello World'
ex5 = '1004Hello'
ex6 = 'Hello~!'

print(ex1.isalpha()) # True
print(ex2.isalpha()) # True
print(ex3.isalpha()) # True
print(ex4.isalpha()) # False
print(ex5.isalpha()) # False
print(ex6.isalpha()) # False
```

## ๐ isdigit()
+ ๋ฌธ์์ด์ ๊ตฌ์ฑ์ด ๋ชจ๋ ์ซ์์ธ์ง ํ์ธํ๋ ํจ์
+ ๊ณต๋ฐฑ์ด๋ ํน์๋ฌธ์๊ฐ ํฌํจ๋๋ฉด False๋ฅผ ๋ฐํ
```python
ex1 = '1'
ex2 = '123'
ex3 = '์๋'
ex4 = 'Hello'
ex5 = '010-1234-5678'
ex6 = '123 456'

print(ex1.isdigit()) # True
print(ex2.isdigit()) # True
print(ex3.isdigit()) # False
print(ex4.isdigit()) # False
print(ex5.isdigit()) # False
print(ex6.isdigit()) # False
```

## ๐ isalnum()
+ ๋ฌธ์์ด์ด ์ํ๋ฒณ ๋๋ ์ซ์์ธ์ง ํ์ธํ๋ ํจ์
+ ๊ณต๋ฐฑ์ด๋ ํน์๋ฌธ์๊ฐ ํฌํจ๋๋ฉด False๋ฅผ ๋ฐํ
```python
ex1 = '123'
ex2 = 'Hello'
ex3 = '123Hello'
ex4 = '123 Hello'
ex5 = '123-Hello'

print(ex1.isalnum()) # True
print(ex2.isalnum()) # True
print(ex3.isalnum()) # True
print(ex4.isalnum()) # False
print(ex5.isalnum()) # False
```
