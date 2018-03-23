# 实验原理

## 量子力学表述

### 原子核自旋

原子核自旋磁矩是其中核子磁矩的总和。
质子自旋为$\dfrac{1}{2}$，自旋磁矩与自旋角动量同向；
而中子自旋为$-\dfrac{1}{2}$，自旋磁矩与自旋角动量反向。由此可知核自旋量子数$I$符合以下规律：偶偶核$I=0$，奇奇核$I$为整数，其它$I$为半整数。核自旋量子数为$I$的原子核核自旋角动量

$$
\boldsymbol{P}_{I} = \sqrt{(I(I+1))}\hbar,
$$

故其核自旋磁矩为

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

### 磁化强度的进动

宏观材料的磁化强度$\boldsymbol{M}=\sum_i{\boldsymbol{\mu}_i}$在磁场中的运动是它内部各原子核磁矩的叠加形成的进动。在静磁场下达到热平衡时，磁化强度中垂直磁场的分量相互抵消，表现为沿磁场方向的$M_0=M_z$。

在$^1_1\mathrm{H}$核，$I=\dfrac{1}{2}$，核磁矩在外磁场中具有的附加能量形成两个磁能级
$$
E_{m_{I}=\frac{1}{2}}=-\dfrac{1}{2}\gamma\hbar B_0,\quad E_{m_I=-\frac{1}{2}}=\dfrac{1}{2}\gamma\hbar B_0.
$$
达到热平衡时，按玻尔兹曼分布估算得到常温下氕核两能级粒子数比约为
$$
\dfrac{N_{20}}{N_{10}}\approx\exp{\dfrac{\Delta E}{kT}}=\exp{\left(-\dfrac{\hbar \gamma B_0}{kT}\right)}=\exp{\left(-\dfrac{\hbar\omega}{kT}\right)}\approx1-\dfrac{\hbar\omega}{kT}=0.999993\approx 1.
$$
故知
$$
M_0 = (N_{10}-N_{20})\mu\approx \dfrac{N\gamma\hbar B_0\mu}{2kT}=\dfrac{N\mu^2}{kT}B_0.
$$
一般地，对核自旋量子数为$I$的物质构成的材料，可以求得平衡态磁化强度
$$
M_0=\dfrac{I+1}{3I}\dfrac{N\mu^2}{kT}B_0=\chi_0 B_0,
$$
其中$\chi_0$为此核的顺次磁化率。

### 弛豫过程

* 横向弛豫（自旋-自旋弛豫）是材料中磁化强度垂直磁场的分量$M_{\perp}$指数衰减的过程。其特征时间$T_2$定义为$M_{\perp}$衰减至初态的$\dfrac{1}{\rm e}$所需的时间。这是由于横向弛豫过程中横向分量的大小衰减速率与分量大小相关：
  $$
  \dfrac{{\rm d}M_x}{{\rm d}t}=-\dfrac{M_x}{T_2},\quad \dfrac{{\rm d}M_y}{{\rm d}t}=-\dfrac{M_y}{T_2}.
  $$
  这一过程来源于不同原子核的自旋磁矩在局部磁场（如核周围的其它粒子产生的磁场）下各自向不同方向偏转，其横向分量的相位逐渐失去相关性，叠加得到的材料磁化强度的横向分量因此逐渐减小。

  由此可知这一过程是通过原子核之间交换能量实现的，所以$T_2$主要与核的性质及所处化学环境相关，可以用于检测材料内部成分。

  液体中的局部磁场一般比固体小很多，所以其横向弛豫时间较长，可达$10^{2-3}$ms。向水中添加顺磁离子（$\mathrm{Cu}^{2+},\mathrm {Fe}^{3+}$等）可以增大局部磁场，缩短其横向弛豫时间。

* 纵向弛豫（热弛豫）是磁化强度平行磁场的分量$M_z$逐渐恢复到与周围环境热平衡时的值$M_0$的过程。其特征时间定义为$M_z-M_0$衰减到原来的$\dfrac{1}{\rm e}$所需的时间。纵向弛豫速率满足方程
  $$
  \dfrac{{\rm d}M_z}{{\rm d}t}=-\dfrac{1}{T_1(M_z-M_0)}.
  $$
  这一过程是通过高能态的核作无辐射跃迁放能，恢复与周围环境的热平衡实现的，所以$T_1$容易受环境温度的影响。

  一般材料中$T_2<T_1$。

  ###布洛赫方程

  磁化强度在磁场中的进动及弛豫过程可以统一用布洛赫方程
  $$
  \dfrac{{\rm d}\boldsymbol{M}}{{\rm d}t} = \gamma\boldsymbol{M}\times\boldsymbol{B}-\dfrac{\hat{\boldsymbol{i}}M_x+\hat{\boldsymbol{j}}M_y}{T_2}-\hat{\boldsymbol{k}}\dfrac{M_z-M_0}{T_1}
  $$
  描述。实验中的横向磁场不是旋转的磁场而是固定方向的水平交变磁场，其产生的线偏振磁场可以分解为左右旋两个分量，由于$^1_1\mathrm{H}$的旋磁比为正，只有其顺时针偏振的分量影响磁化强度的运动。

  ### 稳态解

  取固连于$\boldsymbol{B}_1$且$z'$轴与$z$轴重合的旋转参考系$x'y'z$，设$M_{\perp}$在$x',y'$轴的分量分别为$u,-v$，则由布洛赫方程可得：
  $$
  \begin{cases}
  	\dfrac{{\rm d}u}{{\rm d}t} & = & - &(\omega_0 - \omega)v-\dfrac{u}{T_2}\\
  	\dfrac{{\rm d}v}{{\rm d}t} & = & &(\omega_0 - \omega)u-\dfrac{v}{T_2} & - & \gamma B_1M_z\\
  	\dfrac{{\rm d}M_z}{{\rm d}t} & = & &\dfrac{M_0-M_z}{T_1} & + & \gamma B_1 v
  \end{cases}
  ,\quad (\omega_0 = \gamma B_0)
  $$
  在平衡态下$\dfrac{{\rm d}\boldsymbol{M}}{{\rm d}t}=0$，此时上式的解为稳态解
  $$
  \begin{cases}
      u & = & \dfrac{\gamma T_2^2(\omega_0-\omega)M_0}{1+T_2^2(\omega_0-\omega)^2+\omega_1^2T_1T_2}B_1 & = & \chi'_{\mathrm{R}} B_1,\\
      v & = & \dfrac{\gamma T_2M_0}{1+T_2^2(\omega_0-\omega)^2+\omega_1^2T_1T_2}B_1 & = & \chi'_{\mathrm{I}} B_1,\\
      M_z & = & \dfrac{[1+T_2^2(\omega_0-\omega)]M_0}{1+T_2^2(\omega_0-\omega)^2+\omega_1^2T_1T_2}.
  \end{cases}
  ,\quad (\omega_1 = \gamma B_1, \chi' = \chi'_{\mathrm{R}}+\mathrm{i}\chi'_{\mathrm{I}}\text{是复磁化率}).
  $$

  ## 扫描磁场下的共振信号

   

  ​









.
