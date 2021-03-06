# 实验原理

## 量子力学表述

### 原子核自旋

原子核自旋磁矩是其中核子磁矩的总和。质子自旋为$\dfrac{1}{2}$，自旋磁矩与自旋角动量同向；而中子自旋为$-\dfrac{1}{2}​$，自旋磁矩与自旋角动量反向。由此可知核自旋量子数$I​$符合以下规律：偶偶核$I=0​$，奇奇核$I​$为整数，其它$I​$为半整数。核自旋量子数为$I​$的原子核核自旋角动量

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

​	其中$\omega_0 = |\gamma B_0|, \theta = \left<\boldsymbol{\mu}, \boldsymbol{B}_0\right>$。这表明$\boldsymbol{\mu}$将以拉莫尔频率$\omega_0$绕$\boldsymbol{B}_0$进动；其中$\mu_{\perp}$和$\mu_z$保持不变。

- 时变磁场$\boldsymbol{B}_0 = B_0\hat{\boldsymbol{k}}+B_1(\hat{\boldsymbol{i}}\cos{\omega t} + \hat{\boldsymbol{j}}\sin{\omega t})$下，当横向磁场$\boldsymbol{B}_1$的旋转角频$\boldsymbol{\omega} = \boldsymbol{\omega}_0 = -\gamma \boldsymbol{B}_0$时，因为$\boldsymbol{B}_0$引起的$\boldsymbol{\mu}$的运动是如上节所述的进动，其相当于在与横向磁场固连的以$\boldsymbol{\omega}_0$转动的参考系中静止，即$\dfrac{\partial \boldsymbol{\mu}}{\partial t} = 0$，而同样的转动参考系中由横向磁场引起的运动是核磁矩绕静止的横向磁场的角频率为$\omega_1 = |\gamma B_1|$的章动，所以核磁矩在静止参考系中的运动是绕其横向磁场的进动与横向磁场绕$z$轴的转动的叠加。实验中$B_1\ll B_0$，乘以旋磁比得$\omega_1\ll \omega_0$，故可将横向场的作用效果看作另原有进动锥面上下振荡。

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
其中$\chi_0$为此核的顺磁磁化率。

而在此静磁场上叠加旋转的横向磁场后，磁化强度也将表现出与单核磁矩类似的进动行为；但由于磁矩与磁场平行时能量最低，材料中的所有核磁矩在横向的相位都倾向于保持与$B_1$的转动相位相同，核磁矩间还出现相位相干性。

### 弛豫过程

* 横向弛豫（自旋-自旋弛豫）是材料中磁化强度垂直磁场的分量$M_{\perp}$指数衰减的过程。其特征时间$T_2$定义为$M_{\perp}$衰减至初态的$\dfrac{1}{\rm e}$所需的时间。这是由于横向弛豫过程中横向分量的大小衰减速率与分量大小相关：
  $$
  \dfrac{{\rm d}M_x}{{\rm d}t}=-\dfrac{M_x}{T_2},\quad \dfrac{{\rm d}M_y}{{\rm d}t}=-\dfrac{M_y}{T_2}.
  $$
  这一过程来源于不同原子核的自旋磁矩其横向分量的相位逐渐失去相干性。在$M_{\perp}$横向弛豫的过程中，随着共振频率远离横向磁场振动频率，转动系中表观横向磁场减小，在附近磁场（如核周围的其它原子等离子产生的磁场）的作用下，样品中的原子核自旋磁矩之间交换与旋转磁场的作用能，向不同方向进动，相位逐渐解相干，叠加得到的材料磁化强度的横向分量因此逐渐减小。

  由此可知这一过程是通过原子核之间交换能量实现的，所以$T_2$主要与核的性质及所处化学环境相关，可以用于检测材料内部成分。

  液体中的局部磁场一般比固体小很多，所以其横向弛豫时间较长，可达$10^{2-3}$ms。向水中添加顺磁离子（$\mathrm{Cu}^{2+},\mathrm {Fe}^{3+}$等）可以增大局部磁场，缩短其横向弛豫时间。

* 纵向弛豫（热弛豫）是磁化强度平行磁场的分量$M_z$在共振后逐渐恢复到与周围环境热平衡时的值$M_0$的过程。其特征时间定义为$M_z-M_0$衰减到原来的$\dfrac{1}{\rm e}$所需的时间。纵向弛豫速率满足方程
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


  实验采用连续核磁共振波谱仪（如图）提供纵向扫描磁场和横向射频磁场
$$
(B_0+B'\cos{\omega' t})\hat{\boldsymbol{k}}+B_1\cos{\omega t}\hat{\boldsymbol{i}},
$$
其中垂直磁场的固定分量和交变分量分别由永磁铁和通有50Hz正弦交变电流的扫场线圈$\mathrm{L_m-L'_m}$提供，横向射频磁场则由射频边限振荡器中的电感线圈$\mathrm{L}$提供。

此线圈接在射频边限振荡器中的一个振荡频率可调的谐振电路中，后者中的电流信号一方面经放大后输出到频率计，另一方面其振幅通过检波和放大转化为一个检波输出电平并可通过示波器观察。这一谐振电路的电源振荡频率始终处于它的谐振频率附近；在没有加入试样时，此电路的电流信号为一稳定的简谐电流信号，检波输出电平为一常值，示波器显示为一水平线。实验中，在线圈$\mathrm{L}$中插入试样，调节振荡器谐振频率$\omega_{\rm r}$至
$$
\dfrac{\omega_{\rm r}}{\gamma}\in[B_0-B',B_0+B'],
$$
则在$B_z$振荡的一个周期之内将有两个时刻$t=t_1,t_2$满足$\omega_{\rm r} = \gamma B_z(t)= \omega_0(t)$的条件；这时如果纵向磁场满足慢通过条件，即扫场周期相对弛豫时间足够长$\dfrac{\omega'}{2\pi}\gg T_1$，纵向磁场可以看作是准静态的，那么样品的极化强度$x$分量在这两个时刻附近将按照（ref）变化：
$$
\begin{aligned}
\dfrac{{\rm d}M_x}{{\rm d}t} = & \dfrac{{\rm d}(u\cos{\omega t})}{{\rm d}t}-\dfrac{{\rm d}(v\sin{\omega t})}{{\rm d}t}\\
 = &-\omega B_1\left(\chi'_{\rm R}\sin{\omega t}+\chi'_{\rm I}\cos{\omega t}\right)\\
 = &-\omega B_1|\chi'|\sin{(\omega t+\phi)},
%= & -(\omega_0-\omega)(v\cos{\omega t} + u\sin{\omega t})-\dfrac{u\cos{\omega t} + v\sin{\omega t}}{T_2}+\gamma B_1 M_z\sin\omega t,%\\
%= & \dfrac{M_0}{T_1} - \dfrac{\gamma T_2[T_2(\omega_0-\omega(t))\cos{\omega t}-\sin{\omega t}]M_0/T_1}{1+T_2^2(\omega_0-\omega(t))^2+\omega_1^2T_1T_2}+\dfrac{\gamma^2 T_2M_0}{1+T_2^2(\omega_0-\omega(t))^2+\omega_1^2T_1T_2}B_1^2\\
%= & \dfrac{M_0}{T_1}+\dfrac{\left\{[1+T_2^2(\omega_0-\omega(t))]/T_1+\gamma^2 T_2B_1^2\right\}M_0}{1+T_2^2(\omega_0-\omega(t))^2+\omega_1^2T_1T_2},
\end{aligned}
$$
从而在线圈$\mathrm{L}$中激起与此变化率成正比的感应电动势$\mathscr{E}_{\mathrm{i}}=-\dfrac{\mathrm{d}\mathit{\Phi}_{\mathrm{i}}}{{\rm d}t}\propto-\dfrac{\mathrm{d}M_x}{{\rm d}t}\propto \sin{(\omega t+\phi)}$，其产生的感应电流$I_{\mathrm{i}}\propto \cos{(\omega t+\phi)}$叠加在谐振电路的电流$I_0\propto B_x=B_1\cos{\omega t}$上，使谐振电路发生谐振，总电流振幅变大、振荡器检波输出电平-时间波形上形成一个峰。随着$B_z$的变化，到$\omega_0\approx\omega$时，$\chi_{\rm R}’$可以忽略，所以感应电流的振幅$I_{\rm i,amp}\propto\omega B_1\chi'_{\rm I}\propto v[\omega_0(t)]$；慢通过时短时间内$\omega_0(t)$可以看作线性变化，所以共振峰形状与$v(\omega_0)$相同，为一洛伦兹型峰。此时谐振电路总电动势的频率接近电路的谐振频率，故受到扰动后电路出现谐振，电流振幅变化较大，利于测量。振幅最大时，$\omega_0=\omega\approx\omega_{\rm r}$，频率计示数$\omega$即为核磁共振的频率。

本实验中扫场频率较高，不满足慢通过条件，形成核磁共振后纵向磁场很快偏离$\dfrac{\omega}{\gamma}$，而$M_{\perp}$仍在弛豫过程中，$M_x$的变化不符合稳态解（上式ref），$\dfrac{{\rm d}M_x}{{\rm d}t}$的频率与$\omega$有一个小的差值，感应电流$I_{\rm i}$与谐振电路原有的电流$I_0$叠加后呈现拍频。发生核磁共振时，$\dfrac{{\rm d}M_x}{{\rm d}t}$的频率为$\omega_0$，所以总振幅波动的频率为$2\cdot\dfrac{\omega_0-\omega}{2}=\omega_0-\omega$；同时感应电流的振幅正比于$\dfrac{{\rm d}M_x}{{\rm d}t}$，随着的$M_x$横向弛豫过程的进行$M_x$指数衰减，$I_{\rm i,amp}$也指数衰减。所以共振峰之后输出电平的变化量呈现振幅指数衰减的振荡形状
$$
\Delta I_{\rm total}=\Delta I_{\rm total,0}\exp{\left(-\dfrac{t}{T_2}\right)}\cos{\left[(\omega_0-\omega)t+\phi\right]}.
$$
但实际上连续核磁共振对纵向磁场均匀度的要求很高。因为不同位置的磁感应强度不同会造成样品不同区域的横向磁化强度以不同的速率进动，弥散开来，互相抵消。本实验中的磁场变化幅度$\Delta B^*$（最大与最小磁感应强度之差）对信号衰减的影响远远超过了$M_{\perp}$横向弛豫的影响，测得的衰减常数$T_2^*<T_2$，通常称为表观弛横向豫时间。表观横向弛豫时间满足
$$
\dfrac{1}{T_2^*}=\dfrac{1}{T_2}+\dfrac{\gamma \Delta B^*}{2},
$$
而磁场不均匀度可根据（ref）所示波形的参数表示为
$$
\Delta B^* = \dfrac{2\uppi\omega'\ln{\dfrac{y}{y_0}}}{\omega_0\arcsin{\dfrac{x}{x_0}}}\cdot B_0.
$$
其中$\omega',\omega_0$分别是纵、横向磁场在共振时的圆频率，$x,y,x_0,y_0$分别是某一尾波峰到共振峰的距离、这一尾波峰的对固定电平的高度、共振峰到尾波消失点的距离和共振峰的高度。

## 脉冲磁场下的共振信号

 ### 磁场脉冲

若只在$t_{\rm p}$的短时间内加脉冲磁场$B_1$（不是简谐波），那么转动系中旋磁比为$\gamma$的原子所产生的磁化强度分量$\boldsymbol{M}_{\gamma}$将绕它转动$\theta = \gamma \left({\displaystyle \int}_{-\infty}^{\infty}{B_1\sin{\gamma B_z}t{\rm d}t}\right)\cdot t_{\rm p}$，称为倾倒角。若取$B_1$足够大使得$\theta=90^{\circ}$（或180$^{\circ}$）而且$t_{\rm p}\ll T_2<T_1$（以致这段时间的弛豫过程可忽略），就称此脉冲为90$^{\circ}$脉冲（或180$^{\circ}$脉冲）。脉冲后磁化强度由$M_{\gamma,0}\hat{\boldsymbol{k}}$变为有横向分量，由此开始弛豫则提供横向磁场的横向线圈内即可感应出$M_{\gamma,\perp}$衰减的信号，称为自由感应衰减信号（FID）。由此可见90$^{\circ}$脉冲后FID信号最强而180$^{\circ}$脉冲后恰好没有FID信号。最终的信号是

### 脉冲序列与自旋回波

可以用$90^{\circ}-\tau-180^{\circ}$脉冲序列激发自旋回波。令$t_{\rm p}\ll T_2^*<\tau<T_2<T_1$，则$\boldsymbol{M}$经过90$^{\circ}$脉冲作用后将变为横向，旋转系中恒沿$x'$轴方向，其不同方向的分量将因为纵向磁场的不均匀性而散开，同时各自以较慢的速率发生横向弛豫，不同原子核的磁矩逐渐解相干；这两种效应造成$M_{\perp}$的衰减在横向磁场线圈中激发一个初始幅值为$U(0)$的指数衰减的振荡信号（衰减常数为$T_2^*$）。经过$\tau$（$T_2^*<\tau<T_2$）时间后，不同分量已经充分散开一个角度$\alpha$，每个分量按照它的局域磁场不均匀性的情况决定的方向进动；而不同原子核的磁矩解相干的过程进行得较少。这时再加一180$^{\circ}$脉冲，则不同分量各自绕$x'$轴旋转180$^{\circ}$，夹角变为$360^{\circ}-\alpha$，进动方向和速率不变。于是在$2\tau$时刻，这些分量重新汇合，之后即重复与$0\sim\tau$时段的变化过程，$M_{\perp}$指数衰减的衰减率相同，与横向磁场线圈感应得到一个自旋回波信号；这一时刻磁场不均匀性的影响被抵消，而各原子核磁矩解相干的过程造成的$M_{\perp}$减小进行了一部分，$M_{\perp}(2\tau)=M_{\perp}(0)\exp{\left(-\dfrac{2\tau}{T_2}\right)}$，所以此时的衰减速率是0时刻的$\exp{\left(-\dfrac{2\tau}{T_2}\right)}$倍；故自旋回波的初始峰值
$$
U(2\tau)=U(0)\exp{\left(-\dfrac{2\tau}{T_2}\right)}.
$$
保持$U(0)$不变，测量多组$U(2\tau)-\tau$数据即可拟合出横向弛豫时间$T_2$。

## 化学位移

原子核磁矩的运动还受到附近的电子感应磁场和其它原子的磁场的影响。这些影响可以概括为使原子核实际感受到的磁场比外磁场偏小$\sigma$（屏蔽系数）的比例，即
$$
B_{\rm n}=B_0(1-\sigma).
$$
所以样品中某成分引起的磁化强度的共振频率不仅依赖于其原子的种类，还依赖于其化学环境：
$$
\omega_0=\gamma(1-\sigma)B_0.
$$
一般$\sigma\widetilde{<}10^{-3}$，所以通常用参考物质的屏蔽系数定义样品某种原子核的相对化学位移
$$
\delta=\dfrac{\sigma_{\rm R}-\sigma_{\rm S}}{1-\sigma_{\rm S}}\times10^{6}\approx{(\sigma_{\rm R}-\sigma_{\rm S})}\times10^{6}
$$
来描述该种核的化学环境。