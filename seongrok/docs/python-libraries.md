# 유용한 파이썬 라이브러리 모음

## 내장 함수

- `min(...)`, `max(...)`, `sum(...)`, `eval(수식)`, 
- `sorted([...], reverse=True)`
- `sorted([(), (), ...], key=lambda x: x[1], reverse=True)`
- `int('101', 2)`, `int('707', 8)`, `int('B1E', 16)` - 진법 변환
- `bin(12)[2:]`, `oct(12)[2:]`, `hex(12)[2:]` - 진법 변환

<br/>

## String

- `upper()`, `lower()`, `isupper()`, `islower()`
- 

<br/>

## itertools

반복 데이터, 특히 순열/조합

```python
from itertools import *
a = [1, 2, 3, 4]

b = list(permutations(a, 2)) # 순열
b = list(combinations(a, 2)) # 조합
b = list(product(a, repeat=2)) # 중복 순열
b = list(combinations_with_replacement(a, 2)) # 중복 조합
```

## heapq

우선순위 큐
```python
from collections import deque

queue = deque([1, 2, 3])
queue.append(4)
queue.pop()

while queue:
    pass

```

<br/>


## bisect

Binary Search
```python
from bisect import bisect_left, bisect_right

a = [1, 2, 4, 4, 8]
x = 4

print(bisect_left(a, x))
print(bisect_right(a, x))
```

<br/>


## collections

덱(deque), 카운터(Counter)

- `deque()`: 
- `Counter()`: 각 원소의 개수 카운팅

<br/>


## math

팩토리얼, 제곱근, GCD, LCM, 삼각함수, 파이 등

```python
import math

math.comb()
math.factorial()
```

- `gcd(a, b)`, `lcm(a, b)`
- `ceil()`(올림), `floor()`(내림), `int(), trunc()`(버림), `round()`(반올림)