---
title: "Bell's Inequality"
date: 2024-01-31
author: Jingtian Yu
use_math: true
---

# Quantum correlation

In quantum mechanics, quantum correlation is the expected value of the product of the alternative outcomes. [(Wikipedia)](https://en.wikipedia.org/wiki/Quantum_correlation).

In Bell's 1964 paper, assume two outcomes $A$ and $B$, and each has two outcomes $+1$, $-1$. Then by definition of quantum correlation, first we need "the product of the alternative outcomes": 
\begin{equation\*}
   (+1)\times(+1) = +1,\ (+1)\times(-1) = -1,\ (-1)\times(+1) = -1,\ (-1)\times(-1) = +1
\end{equation\*}

Then the quantum correlation between $A$ and $B$ is
\begin{equation\*}
   \rho_{AB} = P_{++}-P_{+-}-P_{-+}+P_{++}
\end{equation\*}

In an experiment, the estimated quantum correlation is
\begin{equation\*}
   \hat\rho_{AB} = \frac{N_{++}-N_{+-}-N_{-+}+N_{++}}{N_{total}}
\end{equation\*}
where $N_{\cdot\cdot}$ is the observed number of specific combination of $A$ and $B$ outcomes.


# Bell's inequality "in a nutshell"

https://www.zhihu.com/question/55770425/answer/150447979