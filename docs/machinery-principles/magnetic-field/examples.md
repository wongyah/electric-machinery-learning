# 磁路在直流电机中的应用

本节通过三道经典例题，由浅入深地逐步介绍磁路理论在直流电机中是如何应用的。

## 例题：闭合铁芯

![闭合铁芯](https://pic3.zhimg.com/v2-8ba63e64591e0226dc77335c1abf04d6_1440w.jpg "闭合铁芯"){:.standalone}

铁芯的四个边宽度不完全相同：右侧边的宽度为 0.1 m，其余三个边的宽度均为 0.15 m。铁芯的厚度为 0.1 m。铁芯的其它尺寸如图所示。

### 问题

铁芯的左侧边上缠绕着一个 200 匝的线圈。假设铁芯的相对磁导率是 2500，请问每安培输入电流会在铁芯中产生多少磁通量?

### 参考答案

由题义可知，铁芯的横截面积不完全相同：右侧边的横截面积相对较小，其他三个边的横截面积相同。因此，铁芯可以被分成两个区域：

- 右侧边（窄边）
- 其余部分（其他三个边）

该铁芯对应的磁路如下：

![磁路图：闭合铁芯](https://picx.zhimg.com/v2-5756679156ba5e0ef242696a64166029_1440w.jpg "磁路图：闭合铁芯"){:.standalone}

右侧边的平均路径长度 (l~1~) 是 0.45 m，横截面积 (A~1~) 是 0.01 m^2^。因此，右侧边的磁阻可计算如下：

$$
\begin{align*}
  R_{m1} &= \frac{l_1}{\mu A_1} \\
      &= \frac{l_1}{\mu_r \mu_0 A_1} \\
      &= \frac{0.45}{2500 \times (4 \pi \times 10^{-7}) \times 0.01} \\
      &= 14324 \text{ (A/Wb)}
\end{align*}
$$

其余三边的平均路径长度 (l~2~) 是 1.3 m，横截面积 (A~2~) 是 0.015 m^2^。因此，这三个边的磁阻可计算如下：

$$
\begin{align*}
  R_{m2} &= \frac{l_2}{\mu A_2} \\
      &= \frac{l_2}{\mu_r \mu_0 A_2} \\
      &= \frac{1.3}{2500 \times (4 \pi \times 10^{-7}) \times 0.015} \\
      &= 27587 \text{ (A/Wb)}
\end{align*}
$$

铁芯的等效磁阻为：

$$
\begin{align*}
  R_{meq} &= R_{m1} + R_{m2} \\
          &= 14324 + 27587 \\
          &= 41911 \text{ (A/Wb)}
\end{align*}
$$

每安培电流产生的磁动势为：

$$
\begin{align*}
  F_m &= Ni \\
      &= 200 \times 1 \\
      &= 200 \text{ (A)}
\end{align*}
$$

根据[磁路中的欧姆定律]，每安培电流在铁芯中产生的磁通量可计算如下：

$$
\begin{align*}
  \phi &= \frac{F_m}{R_{meq}} \\
       &= \frac{200}{41911} \\
       &= 4.8 \times 10^{-3} \text{ (Wb)}
\end{align*}
$$

## 例题：带气隙的铁芯

![带气隙的铁芯](https://pica.zhimg.com/v2-c2ccc3ac3d7b94ae5937ed5668ae62f6_1440w.jpg "带气隙的铁芯"){:.standalone}

铁芯的平均路径长度是 0.4 m。铁芯的右侧边上有一段长度为 5×10^-4^ m 的气隙 (gas gap)。

铁芯的横截面积是 0.0012 m^2^，相对磁导率是 4000。铁芯左侧边上的缠绕着一个 400 匝的线圈。

### 问题

假设磁场在气隙处产生的边缘效应，使气隙的有效横截面积增加了 5%。请问：

- 整个磁路的等效磁阻是多少?
- 如果要在气隙处产生 0.5 T 的磁通密度，线圈中需要输入多大的电流?

### 参考答案

该铁芯对应的磁路如下：

![磁路图：带气隙的铁芯](https://pic4.zhimg.com/v2-0f6f113e93b239cc82b62f9072ab679f_1440w.jpg "磁路图：带气隙的铁芯"){:.standalone}

根据公式，铁芯的磁阻可计算如下：

$$
\begin{align*}
  R_{mc} &= \frac{l_c}{\mu A_c} \\
      &= \frac{l_c}{\mu_r \mu_0 A_c} \\
      &= \frac{0.4}{4000 \times (4 \pi \times 10^{-7}) \times 0.0012} \\
      &= 66315 \text{ (A/Wb)}
\end{align*}
$$

由于边缘效应，气隙的有效横截面积是铁芯的 1.05 倍。根据公式，气隙的磁阻可计算如下：

$$
\begin{align*}
  R_{ma} &= \frac{l_a}{\mu_0 A_a} \\
      &= \frac{5 \times 10^{-4}}{(4 \pi \times 10^{-7}) \times (0.0012 \times 1.05)} \\
      &= 315784 \text{ (A/Wb)}
\end{align*}
$$

因此，铁芯的等效磁阻为：

$$
\begin{align*}
  R_{meq} &= R_{mc} + R_{ma} \\
          &= 66315 + 315784 \\
          &= 382099 \text{ (A/Wb)}
\end{align*}
$$

> 由于铁芯的磁导率是空气的 4000 倍，虽然气隙的长度仅仅是铁芯的 1/800，但气隙的磁阻却达到铁芯的 5 倍左右。

如果气隙处的磁通密度为 0.5 T，那么磁路中的磁通量可计算如下：

$$
\begin{align*}
  \phi &= BA \\
       &= 0.5 \times (0.0012 \times 1.05) \\
       &= 6.3 \times 10^{-4} \text{ (Wb)}
\end{align*}
$$

根据[磁路中的欧姆定律]，载流线圈应产生的磁动势可计算如下：

$$
\begin{align*}
  F_m &= \phi R_{meq} \\
      &= 6.3 \times 10^{-4} \times 382099 \\
      &= 240.72 \text{ (A)}
\end{align*}
$$

根据公式 (F~m~ = Ni)，载流线圈中的输入电流应为：

$$
\begin{align*}
  i &= \frac{F_m}{N} \\
    &= \frac{240.72}{400} \\
    &= 6.02 \times 10^{-2} \text{ (A)}
\end{align*}
$$

## 例题：直流电机中的铁芯

![直流电机中的铁芯](https://pic4.zhimg.com/v2-032284932e22e340eff614234540b8c5_1440w.jpg "直流电机中的铁芯"){:.standalone}

图中是直流电机中铁芯（定子和转子）的简化模型。定子的平均路径长度为 0.5 m，横截面积为 0.0012 m^2^。转子的平均路径长度为 0.05 m，横截面积也假定为 0.0012 m^2^（与定子相同）。

定子和转子之间存在 5×10^-4^ m 的气隙，气隙的有效横截面积为 0.0014 m^2^（已包含边缘效应的影响）。

### 问题

定子的左侧边上缠绕着一个 200 匝的线圈。铁芯（定子和转子）的相对磁导率是 2000。

如果线圈中的电流为 1 A，请问（定子和转子之间的）气隙中的磁通密度是多少?

### 参考答案

因为气隙的横截面积是已知的，要计算气隙中的磁通密度，只要先知道磁通量就好。要知道磁通量，就得先计算磁动势。而磁动势，只需要按照上文中的第一个例题“闭会铁芯”中的方法求解即可。

直流电机中的铁芯对应的磁路如下：

![磁路图：直流电机中的铁芯](https://picx.zhimg.com/v2-c76681d1de57fa9e9eff43e234f9a9f7_1440w.jpg "磁路图：直流电机中的铁芯"){:.standalone}

定子的磁阻可计算如下：

$$
\begin{align*}
  R_{ms} &= \frac{l_s}{\mu_r \mu_0 A_s} \\
      &= \frac{0.5}{2000 \times (4\pi \times 10^{-7}) \times 0.0012} \\
      &= 165786 \text{ (A/Wb)}
\end{align*}
$$

转子的磁阻可计算如下：

$$
\begin{align*}
  R_{mr} &= \frac{l_r}{\mu_r \mu_0 A_r} \\
      &= \frac{0.05}{2000 \times (4\pi \times 10^{-7}) \times 0.0012} \\
      &= 16579 \text{ (A/Wb)}
\end{align*}
$$

单段气隙的磁阻可计算如下：

$$
\begin{align*}
  R_{ma} &= \frac{l_a}{\mu_0 A_a} \\
      &= \frac{5 \times 10^{-4}}{(4\pi \times 10^{-7}) \times 0.0014} \\
      &= 284205 \text{ (A/Wb)}
\end{align*}
$$

铁芯的等效磁阻为：

$$
\begin{align*}
  R_{meq} &= R_{ms} + R_{mr} + 2R_{ma} \\
          &= 165786 + 16579 + 2 \times 284205 \\
          &= 750775 \text{ (A/Wb)}
\end{align*}
$$

载流线圈产生的磁动势可计算如下：

$$
\begin{align*}
  F_m &= Ni \\
      &= 200 \times 1 \\
      &= 200 \text{ (A)}
\end{align*}
$$

铁芯中的磁通量可以计算如下：

$$
\begin{align*}
  \phi &= \frac{F_m}{R_{meq}} \\
       &= \frac{200}{750775} \\
       &= 2.66 \times 10^{-4} \text{ (Wb)}
\end{align*}
$$

因此线圈中的电流为 1 A 时，气隙中的磁通密度为：

$$
\begin{align*}
  B &= \frac{\phi}{A} \\
    &= \frac{2.66 \times 10^{-4}}{0.0014} \\
    &= 0.19 \text{ (T)}
\end{align*}
$$

## 参考资料

1. Stephen J. Chapman. Electric Machinery Fundamentals: fifth edition. Australia: McGraw-Hill, 2012: 14-21.
2. 汤蕴璆. 电机学: 第五版. 北京: 机械工业出版社, 2014: 9.

<!-- link definition -->

[磁路中的欧姆定律]: ohms-law-in-magnetic-circuit.md