目录见：
http://www.tup.tsinghua.edu.cn/booksCenter/bookcatalog.html?id=04121001
<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=default"></script>
# 同余

## 概念
- 模m的a的剩余类 
$$C_a =   \\{ c | c \in Z, c\equiv a \mod m \\} $$
- 完全剩余系
$$Z/mZ =   \\{ C_a | 0 \le a \le m-1\\} $$
当p为素数
$$F_p = Z/pZ =   \\{ C_a | 0 \le a \le p-1\\} $$
- 简化剩余系
$$(Z/mZ)^* =   \\{ C_a | 0 \le a \le m-1, (a,m) = 1\\} $$
- 欧拉函数
$$ \varphi (p)$$
## 定理
- m_1,m_2,...,m_k互素，x_1,x_2,...,x_k遍历模m_1,m_2,m_3的完全剩余系，则：
$$ (m_2* m_3 * \dots * m_k )*x_1 + \dots + (m_1 * \dots m_{k-1}) * x_k   $$
遍历 m_1 ... m_k 的完全剩余系
- m,n互素：
$$ \varphi (m*n) = \varphi (m) * \varphi (n)$$
用两个剩余系遍历证明
- 
$$\sum_{d | m}{\varphi(d)} = m$$
用d对1,2,...,m分类，每个类的个数为 euler(d),m的总数为m
- 欧拉定理：整数m,(a,m)=1
$$ a^{\varphi (m)} \equiv 1 \mod m$$
最简剩余系乘以a后还是最简剩余系
- 费马小定理
$$ a^p \equiv a \mod p$$
- Wilson 定理:素数p
$$(p-1)! \equiv -1 \mod p$$
2,3...,p-2配对，相乘为1

## 算法
1. 模重复平方算法