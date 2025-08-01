# 安培力与洛伦兹力

无论是[安培环路定律]、[磁路中的欧姆定律]，还是铁磁材料的[磁化曲线]和[磁滞曲线]，都是电生磁过程中的规律和特性。

要说磁场对周围环境或物体的影响力，除了[电磁感应定律]之外，还有安培力和洛伦兹力。所有电机的正常运转都离不开这两种力。

本节将详细说明安培力和洛伦兹力的计算方法，以及判断受力方向的中西手法。


## 安培力

**安培力**是指电流在磁场中受到的力。所有的电机都是利用安培力来工作的。

![通电导线在磁场中受到的安培力](https://pic1.zhimg.com/80/v2-b716d433e0e4991ce35bca7046f4f3b8_720w.webp){:.standalone}

在一个均匀磁场中，有一根导线。磁场的磁通密度为 **B**，磁场方向垂直于屏幕，由外向里。导线的长度是 l，竖直放置（如上图所示）。导线中通有电流，电流大小为 i，方向向下。

由于导线中有电流，周围的磁场就会对导线产生作用力。这个作用力，就是安培力。

安培力的计算公式，如下：

$$
\Large F \normalsize = i \Large ( l \normalsize \times \Large B)
$$

其中，**F** 是安培力（矢量），i 是电流大小，**l** 是导线的长度（矢量，其方向与电流方向一致），**B** 是磁通密度（矢量）。

如果只计算安培力的大小，上式可以简化如下：

$$
F = ilB \sin \theta
$$

其中，θ 是电流方向 (与 **l** 的方向相同) 与磁场方向 (**B** 的方向) 之间的夹角。

## 洛伦兹力

**洛伦兹力**是指运动电荷在磁场中受到的力。

![运动电荷在磁场中受到的洛伦兹力](https://pic3.zhimg.com/80/v2-4746e51cf1e2495494c071e11503581a_720w.webp){:.standalone}

假设导体中单位体积内的电荷数为 n，电荷的带电量和运动速度分别为 q 和 v。导体的横截面积为 S。周围磁场的磁通密度为 **B**。

根照电流的定义，导体中的电流大小可计算如下：

$$
\begin{align*}
  i &= \frac{Q}{t} \\
    &= \frac{Svntq}{t} \\
    &= Svnq
\end{align*}
$$

根据安培力的计算公式，导体在磁场中受到的安培力大小可计算如下：

$$
\begin{align*}
  F_{amp} &= ilB \sin \theta \\
          &= Svnq \times vt \times B \sin \theta \\
          &= Sv^2nqtB \sin \theta
\end{align*}
$$

因此，单个运动电荷在磁场中受到力 —— 洛伦兹力的大小可计算如下：

$$
\begin{align*}
  F_{lor} &= \frac{F_{amp}}{N} \\
        &= \frac{Sv^2nqtB \sin \theta}{Svnt} \\
        &= qvB \sin \theta
\end{align*}
$$

考虑到运动电荷既可以是正电荷也可以是负电荷，如果更严谨一点的话，计算洛伦兹力大小的公式应该写为：

$$
F = |q|vB \sin \theta
$$

由此可见，安培力是洛伦兹力的宏观表现，洛伦兹力是安培力的微观表现。

## 左手定则

要判断安培力和洛伦兹力的方向，使用左手定则：

1. 伸出**左手**，摊平手掌。
2. 使大姆指与其余四个手指垂直。
3. 调整手的方向，**使磁感线从掌心垂直进入，并使四指指向电流的方向（正电荷的运动方向）**。
4. 此时，大姆指所指的方向就是通电导线在磁场中所受安培力（洛伦兹力）的方向。

![左手定则](https://pic3.zhimg.com/80/v2-e00cd503a313499bd41e6833cd3bb78a_720w.webp){:.standalone}

## （西式）右手定则一

在判断安培力和洛伦兹力的方向时，国外通常使用右手定则一：

1. 伸出**右手**，摊平手掌。
2. 使大姆指与其余四个手指垂直。
3. **转动中指使其垂直于手掌，并使无名指和小姆指自然弯曲**。
4. 调整手的方向，使**食指指向电流的方向（正电荷的运动方向），中指指向磁通密度的方向**。
5. 此时，大姆指所指的方向就是通电导线在磁场中所受安培力（洛伦兹力）的方向。

![国外教材中的右手定则一](https://pic4.zhimg.com/80/v2-cae73fed05c940da929460d94dfedbc3_720w.webp "国外教材中的右手定则一"){:.standalone}

由于国内外使用的判断手法不同，叫法也不相同。如果你需要检索外文资料，就得按照国外的习惯输入关键词。否则，你就很难找到想要的内容了。


--8<-- "links.md"
