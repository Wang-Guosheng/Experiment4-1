# 实验原理

## 量子力学表述

### 原子核自旋

原子核自旋磁矩是其中核子磁矩的总和。
质子自旋为$\dfrac{1}{2}$，自旋磁矩与自旋角动量同向；
而中子自旋为$-\dfrac{1}{2}$，自旋磁矩与自旋角动量反向。由此可知**核自旋量子数**$I$符合以下规律：偶偶核$I=0$，奇奇核$I$为整数，其它$I$为半整数。核自旋量子数为$I$的原子核**核自旋角动量**

$$
	\boldsymbol{P}_{I} = \sqrt{(I(I+1))}\hbar,
$$

故其**核自旋磁矩**为

$$
	\boldsymbol{\mu}_{I} = g_N\dfrac{e}{2m_{\text{p}}}\boldsymbol{P}_{I} = g_N\dfrac{e\hbar}{2m_{\text{p}}}\hat{\boldsymbol{\mu}}\_I\sqrt{(I(I+1))} = g_N\boldsymbol{\mu_N}\sqrt{(I(I+1))} = \gamma \boldsymbol{P}_{I}.
$$

式中$g_N$是核的朗德因子，$m_{\text{p}}$为核子质量，$\boldsymbol{\mu_N}$是玻尔磁子，$\gamma$是旋磁比。

###塞曼分裂
在静磁场中，$\boldsymbol{P}_I$的取向量子化，$\boldsymbol{\mu}_I$也随之量子化，

$$
	P_z = m\_I\hbar\Rightarrow \mu_z = \gamma P_z=\gamma m_I\hbar,\quad m_I = I,I-1,\cdots,-I.
$$

由此产生的附加能量和相邻磁能级能量差为

$$
	E = -m_I\gamma\hbar B,\quad \Delta E = \gamma\hbar B = \hbar \omega. (\omega = \gamma B)
$$

## 宏观理论

### 单核拉莫尔进动

在$P_z$量子化的假定下可以得到经典模型

$$
	\dfrac{{\rm d}\boldsymbol{\mu}}{{\rm d}t} = \gamma\dfrac{{\rm d}\boldsymbol{P}}{{\rm d}t} = \gamma (\boldsymbol{\mu}\times \boldsymbol{B})
$$

this
