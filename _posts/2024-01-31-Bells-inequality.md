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

Assume hidden-variable theory [(Wikipedia)](https://en.wikipedia.org/wiki/Hidden-variable_theory) holds, assume one particle is split into two (denote as $A$ and $B$) and flying to opposite direction. Measure the spin of $A$ and $B$ on $xyz$ axes, denote as $(A_x, A_y, A_z)$ and $(B_x, B_y, B_z)$. Then since the conservation of spin on a certain axis, we have $A_i+B_i=0$. Futhermore, since we assume the hidden-variable theory, then we have the following 8 combinations of $(A_x, A_y, A_z, B_x, B_y, B_z)$:

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

Assume the probability of "case $i$" is $P_i$, then by the definitoin of quantum correlation, we have
\begin{equation\*}
\rho_{A_xB_y}=-P_1-P_2+P_3+P_4+P_5+P_6-P_7-P_8
\end{equation\*}
\begin{equation\*}
\rho_{A_xB_z}=-P_1+P_2-P_3+P_4+P_5-P_6+P_7-P_8
\end{equation\*}
\begin{equation\*}
\rho_{A_yB_z}=-P_1+P_2+P_3-P_4-P_5+P_6+P_7-P_8
\end{equation\*}

Notice that
\begin{equation\*}
|\rho_{A_xB_z}-\rho_{A_yB_z}|=2|-P3+P_4+P_5-P_6|=2|(P_4+P_5)-(P_3+P_6)|\leq2(|P_4+P_5|+|P_3+P_6|)
\end{equation\*}
also notice that all $P_i$ are positive, and $\sum_iP_i=1$ then
\begin{equation\*}
2(|P_4+P_5|+|P_3+P_6|)=2(P_3+P_4+P_5+P_6)
\end{equation\*}
\begin{equation\*}
=1+(-P_1-P_2+P_3+P_4+P_5+P_6-P_7-P_8)=1+\rho_{A_xB_y}
\end{equation\*}

In summary, we have
\begin{equation\*}
|\rho_{A_xB_z}-\rho_{A_yB_z}|\leq1+\rho_{A_xB_y}
\end{equation\*}

Or write it in a more commonly seen way:
\begin{equation\*}
|P_{xz}-P_{zy}|\leq1+P_{xy}
\end{equation\*}