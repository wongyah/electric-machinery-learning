# 定轴转动中的功和功率

功率是很多设备的关键技术指标，代表着设备的“能力”大小。小到电饭煲、电磁炉，大到飞机、航空母舰的发动机，“它的功率多大”总是成为买家或看客最为关注的问题之一。

结合直线运动中功和功率的概念，我们一起来看看旋转运动中功和功率。

## 功

功（W）表示能量转化的多少。如果一个物体受到力的作用，并在力的方向上发生了位移，那么这个力就对物体做了功。

![日常生活中关于“功”的例子](https://picx.zhimg.com/v2-4969a12982628d4a9c70a3414258ec2b_1440w.jpg "日常生活中关于“功”的例子"){:.standalone}

假设物体发生位移的方向与力的方向一致，功的大小可以计算如下：

$$
\begin{equation}
  W = \int F \ \mathrm{d}r
\end{equation}
$$

其中，W 是力对物体所做的功，F 是作用在物体上的力，r 是物体在力的方向上发生的位移。

如果力的大小是恒定不变的，上式可以简化为：

$$
W = Fr
$$

在旋转运动中，如果一个物体受到扭矩的作用而发生了转动，那么这个扭矩也对物体做了功。功的大小可以计算如下：

$$
\begin{equation}
  W = \int \tau \ \mathrm{d}\theta
\end{equation}
$$

其中，τ 是作用在物体上的扭矩，θ 是物体转动的角度。

如果扭矩的大小是恒定不变的，上式可以简化为：

$$
W = \tau \theta
$$

在国际单位制中，功的度量单位是焦耳 (J)。

## 功率

功率 (P) 表示做功的快慢，或者单位时间内对物体做的功。功率的计算公式如下：

$$
\begin{equation}
  P = \frac{\mathrm{d}W}{\mathrm{d}t}
\end{equation}
$$

其中，P 是功率，W 是力对物体做的功，t 是做功所用的时间。

如果物体发生位移的方向与力的方向一致，且力的大小是恒定不变的，上式可以简化为：

$$
\begin{align*}
P &= \frac{\mathrm{d}W}{\mathrm{d}t} \\
  &= \frac{\mathrm{d}}{\mathrm{d}t} (Fr) \\
  &= F \bigg(\frac{\mathrm{d}r}{\mathrm{d}t}\bigg) \\
  &= Fv
\end{align*}
$$

其中，v 是物体运动的速度。

同理，如果扭矩的大小是恒定不变的，旋转运动中功率的计算公式如下：

$$
\begin{align*}
P &= \frac{\mathrm{d}W}{\mathrm{d}t} \\
  &= \frac{\mathrm{d}}{\mathrm{d}t} (\tau\theta) \\
  &= \tau \bigg(\frac{\mathrm{d}\theta}{\mathrm{d}t}\bigg) \\
  &= \tau\omega
\end{align*}
$$

即：

$$
\begin{equation}
  P = \tau\omega
\end{equation}
$$

其中，ω 是物体转动的角速度。

在国际单位制中，功率的度量单位是焦耳/秒 (J/s)，也叫做瓦特 (W)。

在上式中，功率的单位是瓦特 (W)，扭矩的单位是牛顿·米 (N·m)，角速度的单位是弧度/秒 (rad/s)。

旋转运动的功率计算公式可以用来计算电动机或发电机的功率，是电机学中最重要的内容之一。


