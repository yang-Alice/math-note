# Sample spaces 样本空间
**Definition** (Sample space and event). The sample space $S$ of an experiment is the set of all possible outcomes of the experiment. An event $A$ is a subset of the sample space $S$, and we say that A occurred if the actual outcome is in $A$.

**定义**：每一个概率模型都关联着一个试验,这个试验将产生一个试验结果. 该试验的所有可能结果形成样本空间,用$S$表示样本空间.样本空间的子集,即某些试验结果的集合,称为事件$A$

# Probability 概率
## Probability 概率定义
**Definition** (Probability). The probability of an event $A$ is a number $P(A)$, which is a nonnegative real number such that $0 \leq P(A) \leq 1$.+

(General definition of probability). A probability space consists of a sample space $S$ and a probability function $P$ which takes an event $A ⊆ S$ as input and returns $P(A)$, a real number between 0 and 1, as output. The function $P$ must satisfy the following axioms:
1. $P(∅) = 0, P(S) = 1.$
2. If $A1$, $A2$, . . . are disjoint events, then
$$P\left(\bigcup_{j=1}^{\infty}A_j\right) = \sum_{j=1}^{\infty}P(A_j)$$

(Saying that these events are disjoint means that they are mutually exclusive: $Ai ∩ Aj = ∅$ for $i \ne j$.)

## Random variables 随机变量
**Definition** (Random variable). Given an experiment with sample space $S$, a random variable (r.v.) is a function from the sample space $S$ to the real numbers \mathbb{R}. It is common, but not required, to denote random variables by capital letters.

随机变量的缩写是r.v.

**Definition** (Discrete random variable) 离散随机变量

A random variable $X$ is said to be discrete if there is a finite list of values $a1, a2, . . . ,$ an or an infinite list of values $a1, a2, . . .$ such that $P(X = a_j \text{ for some }  j) = 1$. If $X$ is a discrete r.v., then the finite or countably infinite set of values $x$ such that $P(X = x) > 0$ is called the support of $X$.

**Definition** (Continuous r.v.). 

An r.v. has a continuous distribution if its CDF(cumulative distribution function) is differentiable. We also allow there to be endpoints (or finitely many points) where the CDF is continuous but not differentiable, as long as the CDF is differentiable everywhere else. A continuous random variable is a random variable with a continuous distribution.

## Probability mass function 概率质量函数
**Definition** (Probability mass function). The probability mass function(PMF) of a discrete r.v. X is the function pX given by $p_X(x) = P(X = x)$. Note that this is positive if $x$ is in the support of $X$, and 0 otherwise

## cumulative distribution function 累积分布函数
**Definition** The cumulative distribution function (CDF) of an r.v. $X$ is the function $F_X$ given by $F_X(x) = P(X ≤ x)$. When there is no risk of ambiguity, we sometimes drop the subscript and just write $F$ (or some other letter) for a CDF.

## Functions of random variables

**Definition** (Function of an r.v.). For an experiment with sample space $S$, an r.v. $X$, and a function $g : R → R$ , $g(X)$ is the r.v. that maps $s$ to $g(X(s))$ for all $s ∈ S$.


**Definition** (Function of two r.v.s). 

Given an experiment with sample space $S$, if $X$ and $Y$ are r.v.s that map $s ∈ S$ to $X(s)$ and $Y(s)$ respectively, then $g(X, Y)$ is the r.v. that maps $s$ to $g(X(s), Y(s))$.


**Definition** (Independence of many r.v.s). 

Random variables $X1, . . . , Xn$ are independent if $P(X_1 ≤ x_1, . . . , X_n ≤ x_n) = P(X_1 ≤ x_1)\times. . . \times P(X_n ≤ x_n)$, for all $x_1, . . . , x_n ∈ R$. For infinitely many r.v.s, we say that they are independent if every finite subset of the r.v.s is independent.

**Definition**  Definition 3.8.6 (i.i.d.). 

We will often work with random variables that are independent and have the same distribution. We call such r.v.s independent and identically distributed, or i.i.d. for short.

## Continuous random variables 连续随机变量
**Definition** Continuous random variables

An r.v. has a continuous distribution if its CDF(cumulative distribution function) is differentiable. We also allow there to be endpoints (or finitely many points) where the CDF is continuous but not differentiable, as long as the CDF is differentiable everywhere else. A continuous random variable is a random variable with a continuous distribution.

**Definition** (Probability density function). 概率密度函数

The probability density function (PDF) of a continuous r.v. $X$ is the function $f_X$ given by $f_X(x) = \frac{d}{dx}F_X(x)$, where $F_X$ is the CDF of $X$. Note that $f_X(x)$ is positive if $x$ is in the support of $X$, and 0 otherwise.