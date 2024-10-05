
**定理**

数列 $\displaystyle a_{n}$ 有有限极限的充要条件是 : 对于 $\displaystyle \forall\varepsilon>0,\exists N \in \mathbb{N}_{+},\,s.t.\,n>N及n'>N$ 时，有
$$
\left | a_{n}-a_{n'}\right |<\varepsilon. 
$$

**证明:**

**必要性**

设 $\displaystyle a_{n}$ 有有限极限 $\displaystyle a.$ 
对于 $\displaystyle \forall\varepsilon>0,\exists N \in \mathbb{N}_{+},\,s.t.\,n>N及n'>N$ 同时成立
$$
\left | a_{n}-a \right |< \frac{\varepsilon}{2}\quad,\quad \left | a-a_{n'} \right |< \frac{\varepsilon}{2} 
$$
由此
$$
\left | a_{n} -a_{n'}\right |=\left |(a_{n}-a) -(a-a_{n'}) \right | \leqslant\left | a_{n}-a \right |+\left | a-a_{n'} \right |=\varepsilon.  
$$
**充分性**

首先假设 $\displaystyle a_{n}$ 收敛 , 即 $\displaystyle \lim\limits_{ n \to {\infty} }a_{n}=a$ ,则其子数列 $\displaystyle a_{n_{k}}$ , 亦收敛于 $\displaystyle a$ , 故 $\displaystyle \exists K$ , 当 $\displaystyle k>K$ 时有
$$
\left | a_{n_{k}}-a \right | < \frac{\varepsilon}{2}  
$$
当 $\displaystyle n>N及n'>N$ 同时成立时 , 有
$$
\left | a_{n}-a_{n'} \right |<\varepsilon\implies\left | a_{n}-a_{n'}\right |< \frac{\varepsilon}{2}  
$$
取 $\displaystyle M=\max \left \{  N, K\right \}$
因 $\displaystyle n_{k}\geqslant k$ , 当 $\displaystyle k\geqslant M$ 时 , $\displaystyle n_{k}\geqslant N,n_{k}\geqslant K$ , 故
$$
\left | a_{n}-a \right |=\left | a_{n}-a_{n_{k}}+a_{n_{k}}-a \right |\leqslant \left | a_{n}-a_{n_{k}} \right |+\left | a_{n_{k}}-a \right |< \frac{\varepsilon}{2}+ \frac{\varepsilon}{2}=\varepsilon    
$$
故 $\displaystyle a_{n}$ 收敛 , 假设成立.