## π Counter() ν΄λμ€
+ collections λͺ¨λμμ μ κ³΅νλ ν΄λμ€
+ μ¬μ (dict) ν΄λμ€μ νμ ν΄λμ€
+ λ¦¬μ€νΈλ ννμμ κ° λ°μ΄ν°κ° λ±μ₯ν νμλ₯Ό ```μ¬μ  νμ```μΌλ‘ λ°ν
+ κ°μ₯ λ§μ΄ λ±μ₯ν κ°λΆν° λ΄λ¦Όμ°¨μμΌλ‘ λ°ν

```python
from collections import Counter

list = [4, 4, 6, 5, 7, 7, 7, 8]
ct = Counter(list)
print(ct)

# Counter({7: 3, 4: 2, 6: 1, 5: 1, 8: 1})
```
```python
from collections import Counter

colors = ['red', 'blue', 'red', 'green', 'blue', 'blue']
ct = Counter(colors)
print(ct)

# Counter({'blue': 3, 'red': 2, 'green': 1})
```

### π‘ Counter ν΄λμ€μ most_common() λ©μλ
+ Counter()μ κ²°κ³Όκ°μ λ΄λ¦Όμ°¨μμΌλ‘ μ λ¦¬νμ¬ λ¦¬μ€νΈ μμ ννλ‘ λ°ν
+ μΈμμ μ«μλ₯Ό λ£μΌλ©΄ ν΄λΉνλ μλ§νΌ μμ κ²°κ³Όκ°λΆν° λ°ν

```python
from collections import Counter

list = [4, 4, 6, 5, 7, 7, 7, 8]
ct = Counter(list)

mc = ct.most_common()
print(mc)

mc = ct.most_common(1) # μμ κ²°κ³Όκ° 1κ°λ§ λ°ν
print(mc)

# [(7, 3), (4, 2), (6, 1), (5, 1), (8, 1)]
# [(7, 3)]
```

```python
from collections import Counter

colors = ['red', 'blue', 'red', 'green', 'blue', 'blue']
ct = Counter(colors)

mc = ct.most_common()
print(mc)

mc = ct.most_common(2) # μμ κ²°κ³Όκ° 2κ°λ§ λ°ν
print(mc)

# [('blue', 3), ('red', 2), ('green', 1)]
# [('blue', 3), ('red', 2)]
```

μ°Έκ³ : https://codepractice.tistory.com/71
