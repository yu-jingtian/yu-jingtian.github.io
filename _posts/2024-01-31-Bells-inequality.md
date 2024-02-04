---
title: "Bell's Inequality"
date: 2024-01-31
author: Jingtian Yu
use_math: true
---

# Quantum correlation

In quantum mechanics, quantum correlation is the expected value of the product of the alternative outcomes. [(Wikipedia)](https://en.wikipedia.org/wiki/Quantum_correlation).

In Bell's 1964 paper, assume two outcomes $O_1$ and $O_2$, and each has two outcomes $+1$, $-1$. Then by definition of quantum correlation, first we need "the product of the alternative outcomes": 
\begin{equation\*}
   (+1)\times(+1) = +1,\ (+1)\times(-1) = -1,\ (-1)\times(+1) = -1,\ (-1)\times(-1) = +1
\end{equation\*}

Then the quantum correlation between $A$ and $B$ is
\begin{equation\*}
   \rho_{O_1O_2} = P_{++}-P_{+-}-P_{-+}+P_{++}
\end{equation\*}

In an experiment, the estimated quantum correlation is
\begin{equation\*}
   \hat\rho_{O_1O_2} = \frac{N_{++}-N_{+-}-N_{-+}+N_{++}}{N_{total}}
\end{equation\*}
where $N_{\cdot\cdot}$ is the observed number of specific combination of $O_1$ and $O_2$ outcomes.


# Bell's inequality "in a nutshell"

Assume hidden-variable theory [(Wikipedia)](https://en.wikipedia.org/wiki/Hidden-variable_theory) holds, assume one particle is split into two (denote as $A$ and $B$) and flying to opposite direction. Measure the spin of $A$ and $B$ on $xyz$ axes, denote as $(A_x, A_y, A_z)$ and $(B_x, B_y, B_z)$. Then since the conservation of spin on a certain axis, we have $A_\cdots+B_\cdots=0$. Futhermore, since we assume the hidden-variable theory, then we have the following 8 combinations of $(A_x, A_y, A_z, B_x, B_y, B_z)$:

|        | Ax | Ay | Az | Bx | By | Bz |
|--------|----|----|----|----|----|----|
| case 1 | +  | +  | +  | -  | -  | -  |
| case 2 | +  | +  | -  | -  | -  | +  |
| case 3 | +  | -  | +  | -  | +  | -  |
| case 4 | +  | -  | -  | -  | +  | +  |
| case 5 | -  | +  | +  | +  | -  | -  |
| case 6 | -  | +  | -  | +  | -  | +  |
| case 7 | -  | -  | +  | +  | +  | -  |
| case 8 | -  | -  | -  | +  | +  | +  |
