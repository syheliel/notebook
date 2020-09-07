
# 自动机
## 有限状态自动机(DFA)
DF𝐴=(𝑄,Σ,𝛿,$𝑞_0$,𝐹)
𝑄 is a finite set of states
Σ is a finite set of input symbols
𝛿:𝑄×Σ→𝑄 is a transition function
$𝑞_0$ is a start state
𝐹 is a set of final (accepting) states 

## 不确定的有限状态自动机(NFA)
𝑁𝐹𝐴=(𝑄,Σ,𝛿,$𝑞_0$,𝐹)
𝑄 is a finite set of state
Σ is a finite set of input symbols
𝛿:𝑄×Σ→2^𝑄 is a transition function
$𝑞_0$ is a start state
𝐹 is a set of final (accepting) states

## NFA和DFA的等价性
构造法：
对NFA $(𝑄_𝑁, \sum , \delta_𝑁, 𝑞_0,𝐹_𝑁)$
构造DFA$𝐷=(𝑄_𝐷,Σ,\delta_𝐷,\{𝑞_0\},𝐹_𝐷)$
$𝑄_𝐷=\{𝑆|𝑆 \subseteq 𝑄_𝑁\}$    
𝐹_𝐷={𝑆┤|𝑆⊆𝑄_𝑁∧𝑆∩𝐹_𝑁≠∅} 
For any 𝑆⊆𝑄_𝑁 and input symbol 𝑎∈Σ,
$$\delta_D(𝑆,𝑎)=⋃_{𝑝 \in 𝑆}\delta_𝑁 (𝑝,𝑎)$$
## 带空迁移的有限自动机𝜖-NFA
𝜖-NFA(𝑄,Σ,𝛿,𝑞_0,𝐹)
𝑄 is a finite set of state
Σ is a finite set of input symbols
𝛿:𝑄×Σ∪{𝜖}→2^𝑄 is a transition function
𝑞_0 is a start state
𝐹 is a set of final (accepting) states