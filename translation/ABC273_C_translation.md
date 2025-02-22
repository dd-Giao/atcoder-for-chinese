## 题意

给出一个长度为 $N$ 的序列 $A$，对于每一个 $K \in [0,N-1]$，解决如下问题：

> 找出在 $[1,N]$ 之间的符合以下条件的 $i$ 的数量：
>
> - 序列 $A$ 中刚好有 $K$ 种数大于 $A_i$。

## 数据范围

- $1 \leq N < 2 \times 10^5$

- $1 \leq A_i \leq 10^9$

- 所有输入均为整数。

## 输入格式

第一行输入一个整数 $N$，表示序列长度。

第二行输入 $N$ 个整数 $A_i$，表示序列的值。

## 输出格式

输出共 $N$ 行，第 $i$ 行为 $K=i-1$ 时的答案。

## 样例

### 样例输入1

```
6
2 7 1 8 2 8
```

### 样例输出1

```
2
1
2
1
0
0
```

### 样例解释1

以 $K=2$ 为例：

- 序列 $A$ 中有 $2$ 种数大于 $A_1$： $7,8$。

- 序列 $A$ 中有 $1$ 种数大于 $A_2$： $8$。

- 序列 $A$ 中有 $3$ 种数大于 $A_3$： $2,7,8$。

- 序列 $A$ 中没有数大于 $A_4$。

- 序列 $A$ 中有 $2$ 种数大于 $A_5$： $7,8$。

- 序列 $A$ 中没有数大于 $A_6$。

当 $i=1$ 或 $i=5$ 时序列 $A$ 中刚好有 $K$ 种数大于 $A_i$，所以答案为 $2$。

### 样例输入2

```
1
1
```

### 样例输出2

```
1
```

### 样例输入3

```
10
979861204 57882493 979861204 447672230 644706927 710511029 763027379 710511029 447672230 136397527
```

### 样例输出3

```
2
1
2
1
2
1
1
0
0
0
```
