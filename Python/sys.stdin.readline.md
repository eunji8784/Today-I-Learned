## ๐ก sys.stdin.readline()
+ input()๊ณผ ๊ฐ์ ํ์ด์ฌ ์๋ ฅ ๋ฐฉ์ ์ค ํ๋ (* _input(): ํ์ด์ฌ์์ ์ ๊ณตํ๋ ๋ด์ฅ ํจ์_)
+ ๋ฐ๋ณต๋ฌธ์ผ๋ก ์ฌ๋ฌ ์ค ์๋ ฅ๋ฐ๋ ๊ฒฝ์ฐ input()์ ์๊ฐ์ด๊ณผ๊ฐ ๋ฐ์ํ  ์ ์์
+ return ํ์์ __๋ฌธ์์ด__
+ ์๊ฐ์ด๊ณผ ๋ฐฉ์ง๋ฅผ ์ํด ```sys.stdin.readline()```์ผ๋ก ์ฐ๋ ์ต๊ด์ ๋ค์ด์
```
- sys ๋ชจ๋์ Python ์ธํฐํ๋ฆฌํฐ๊ฐ ์ ๊ณตํ๋ ๋ณ์์ ํจ์๋ฅผ ์ง์  ์ ์ดํ  ์ ์๊ฒ ํด์ฃผ๋ ๋ชจ๋
- stdin์ Python ์ธํฐํ๋ฆฌํฐ๊ฐ ํ์ค ์๋ ฅ์ ์ฌ์ฉํ๋ ํ์ผ ๊ฐ์ฒด, readline()์ ํ์ผ ๊ฐ์ฒด์ ๋ฉ์๋ ์ค ํ๋๋ก read(), readlines() ์ ๊ฐ์ด ํ์ผ ๊ฐ์ฒด๋ฅผ ์ฝ์ ๋ ์ฌ์ฉ

์ฆ, sys.stdin.readline() ์ sys ๋ผ๋ ๋ชจ๋์ ํ์ผ ๊ฐ์ฒด stdin ์ ๋ฉ์๋ ์ค readline() ์ ์ฌ์ฉํ๋ค๋ ์๋ฏธ์ด๋ค
readline() ์ ์๋ ฅ์ ์ฝ์ ๋ ํ ๋ฒ์ ํ ์ค์ฉ ์ฝ๋๋ฐ, ์ด ๋ง์ ์ฌ๋ฌ ์ค์ ์๋ ฅ์ด ์์ ๋ ํ ์ค์ ์ฝ๊ณ  ๋๋ฉด ๊ทธ ๋ค์ ์ค์ ๊ฐ๋ฆฌํจ๋ค๋ ๋ป
```
์ถ์ฒ: https://velog.io/@ecvheo1/%EC%9E%85%EB%A0%A5-%EB%B0%9B%EB%8A%94-%EB%B0%A9%EB%B2%95-sys.stdin.readline, https://developeryuseon.tistory.com/90


### ๐ ์ ์ ์๋ ฅ๋ฐ์ ๋ int๋ก ๋ณํ ํ์
+ ```sys.stdin.readline()```์ ํ ์ค ๋จ์๋ก ์๋ ฅ๋ฐ๊ธฐ ๋๋ฌธ์ ๊ฐํ๋ฌธ์๊ฐ ๊ฐ์ด ํฌํจ๋จ. _ex) 3 -> 3\n_
```python
import sys
n = int(sys.stdin.readline())
```
+ ์ ์ํ ๋ณํ๊ณผ ํจ๊ป ๊ฐํ๋ฌธ์๋ ์ ๊ฑฐ๋จ

### ๐ n์ค์ ๋ฌธ์์ด์ ์๋ ฅ๋ฐ์ ๋ฆฌ์คํธ์ ์ ์ฅํ๋ ๊ฒฝ์ฐ
+ ```strip()```์ผ๋ก ๋ฌธ์์ด ๋งจ ์ผ์ชฝ๊ณผ ์ค๋ฅธ์ชฝ์ ๊ณต๋ฐฑ๋ฌธ์๋ฅผ ์ ๊ฑฐ
```python
import sys
n = int(sys.stdin.readline())
data = [sys.stdin.readline().strip() for _ in range(n)]
```

#### โ strip()
+ ```strip([chars])``` : ์ธ์๋ก ์ ๋ฌ๋ ๋ฌธ์๋ฅผ String์ ์ผ์ชฝ๊ณผ ์ค๋ฅธ์ชฝ์์ ์ ๊ฑฐ
+ ```lstrip([chars])``` : ์ธ์๋ก ์ ๋ฌ๋ ๋ฌธ์๋ฅผ String์ ์ผ์ชฝ์์ ์ ๊ฑฐ
+ ```rstrip([chars])``` : ์ธ์๋ก ์ ๋ฌ๋ ๋ฌธ์๋ฅผ String์ ์ค๋ฅธ์ชฝ์์ ์ ๊ฑฐ
