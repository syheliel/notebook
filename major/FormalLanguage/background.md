#形式语言
## 定义
L =$(\sum,G)$
Alphabet: Σ
Grammar: 𝐺 
## 语法
𝐺=(𝑉,𝑇,𝑃,𝑆)
V: set of syntactic variables, nonterminal symbols
T: set of terminal symbols
P: set of production 𝛼→𝛽 where 𝛼∈(𝑉∪𝑇)^+, 𝛽∈(𝑉∪𝑇)^∗
S: start symbol 𝑆∈𝑉
例子：
𝐺_3=({𝐴,𝐵},{0,1},{𝐴→01|0𝐴1|1𝐴0 , 𝐵→𝐴𝐵|0},𝐴)
## 推导方向
- 最左推导：在推导过程中总是替换句子最左端的非终止符号
- 最右推导：在推导过程中总是替换句子最右端的非终止符号
- 任意推导：既不是最左推导也不是最右推导
一个语句的不同推导对应于相同的推导树
一个语句的推导树和其最左推导之间满足双射关系

## 文法分类：
- 0型文法：由文法结构定义的文法，也叫递归可枚举文法（recursively enumerable）
- 1型文法：（context-sensitive）
For every 𝛼𝐴𝛽→𝛼𝛾𝛽, 𝛼,𝛽∈$(𝑉∪𝑇)^∗$, 𝐴∈𝑉 and 𝛾∈$(𝑉∪𝑇)^+$
- 2型文法：（context-free）
For every 𝐴→𝛽, 𝐴∈𝑉 and 𝛽∈$(𝑉∪𝑇)^∗$
- 3型文法：（regular）
Every production is of the form 𝐴→𝜎𝐵 or 𝐴→𝜎 where 𝐴,𝐵∈𝑉 and 𝜎∈$𝑇^∗$
0型⊃1型⊃2型⊃3型