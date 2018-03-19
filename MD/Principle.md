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

考虑两种磁场：

- 静磁场$\boldsymbol{B}_0 = B_0\hat{\boldsymbol{k}}$下，方程化为

$$
	\begin{cases}
		\dfrac{{\rm d}^2\mu_x}{{\rm d}t^2} & + \gamma^2B_0^2\mu_x & = 0\\
		\dfrac{{\rm d}^2\mu_y}{{\rm d}t^2} & + \gamma^2B_0^2\mu_y & = 0\\
		\dfrac{{\rm d}\mu_z}{{\rm d}t} & & = 0
	\end{cases}
	\Rightarrow
	\begin{cases}
		\mu_x = \mu \sin{\theta}\sin{\left(\omega_0 t + \delta\right)}\\
		\mu_y = \mu \sin{\theta}\sin{\left(\omega_0 t + \delta\right)}\\
		\mu_z = \mu \cos{\theta}
	\end{cases},
$$

其中$\omega_0 = |\gamma B_0|, \theta = \left<\boldsymbol{\mu}, \boldsymbol{B}_0\right>$。这表明$\boldsymbol{\mu}$将以拉莫尔频率$\omega_0$绕$\boldsymbol{B}_0$进动；其中$\mu_{\perp}$和$\mu_z$保持不变。

- 时变磁场$\boldsymbol{B}_0 = B_0\hat{\boldsymbol{k}}+B_1(\hat{\boldsymbol{i}}\cos{\omega_0 t} + \hat{\boldsymbol{j}}\sin{\omega_0 t})$下，如果横向磁场$\boldsymbol{B}_1$的旋转角频$\boldsymbol{\omega}_0 = -\gamma \boldsymbol{B}_0$，那么因为$\boldsymbol{B}_0$引起的$\boldsymbol{\mu}$的运动是如上节所述的进动，其相当于在与横向磁场固连的以$\boldsymbol{\omega}_0$转动的参考系中静止，即$\dfrac{\partial \boldsymbol{\mu}}{\partial t} = 0$，而同样的转动参考系中由横向磁场引起的运动是核磁矩绕静止的横向磁场的角频率为$\omega_0 = |\gamma B_1|$的进动，所以核磁矩在静止参考系中的运动是绕其横向磁场的进动与横向磁场绕$z$轴的转动的叠加。实验中$B_1\ll B_2$，乘以旋磁比得$\omega_1\ll \omega_0$，故可横向场的作用效果看作另原有进动锥面上下振荡。
