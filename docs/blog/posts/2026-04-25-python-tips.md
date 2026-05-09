---
date: 2026-04-25
categories:
  - python
tags:
  - python
  - 技巧
authors:
  - your-name
slug: python-tips
---

# 每个开发者都应该知道的 5 个 Python 技巧

以下是五个能让你的代码更简洁、更高效的 Python 技巧。

<!-- more -->

## 1. 使用列表推导式

```python
# 以前这样写：
squares = []
for x in range(10):
    squares.append(x**2)

# 现在这样写：
squares = [x**2 for x in range(10)]
```

## 2. 善用 f-String

```python
name = "世界"
print(f"你好，{name}！")  # 你好，世界！
```

## 3. 轻松解包

```python
first, *middle, last = [1, 2, 3, 4, 5]
print(first)   # 1
print(middle)  # [2, 3, 4]
print(last)    # 5
```

## 4. 使用 `zip` 配对迭代

```python
names = ["张三", "李四", "王五"]
scores = [85, 92, 78]

for name, score in zip(names, scores):
    print(f"{name}：{score}")
```

## 5. 海象运算符（`:=`）

```python
# Python 3.8+
if (n := len(data)) > 10:
    print(f"数据太长了：共 {n} 项")
```

---

这些小技巧积累起来，能大幅提升代码的可读性和效率。
