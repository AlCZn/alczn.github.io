# AlCZn 的第一个博客！！！

## 一、段落与排版

一个 Markdown 段落是由一个或多个连续文本行组成，前后需要有空行。

在行末输入两个空格或一个反斜杠（`\`），可以实现比分段更加紧凑的换行效果：

这是第一行文本  
这是通过行末两个空格换行的第二行

这是第三行文本\
这是通过行末反斜杠换行的第四行

### 强调与修饰
- *单星号斜体* 与 _单下划线斜体_
- **双星号加粗** 与 __双下划线加粗__
- ***粗斜体文本***
- ~~删除线文本~~
- 转义符号演示：\*不是斜体\*、\[不是链接\]、\$不是公式\$

---

## 二、代码块（带行号与高亮）

洛谷代码块默认会 fallback 到 C++，同时支持 `line-numbers`（显示行号）和 `lines=start-end`（指定行高亮）：

```cpp line-numbers lines=7-10
#include <iostream>
#include <vector>
#include <algorithm>
using namespace std;

int main() {
    ios::sync_with_stdio(false);
    cin.tie(nullptr);
    
    int n;
    if (!(cin >> n)) return 0;
    cout << "Hello, Luogu! n = " << n << endl;
    return 0;
}
```

---

## 三、LaTeX 与 KaTeX 数学公式支持

洛谷使用 KaTeX 进行公式渲染，支持行内公式 `$ ... $` 和行间公式 `$$ ... $$`。

行内公式示例：对于任意的 $x, y \in \mathbb{R}$，均有 $(x + y)^2 = x^2 + 2xy + y^2$。

行间公式示例（多行对齐与微积分）：

$$
\begin{aligned}
\int_{0}^{+\infty} e^{-x^2} \mathrm{d}x &= \frac{\sqrt{\pi}}{2} \\
H_n &= \sum_{i = 1}^{n} \frac{1}{i} \sim \ln n + \gamma + \mathcal{O}\left(\frac{1}{n}\right)
\end{aligned}
$$

分段函数与矩阵：

$$
f(x) = \begin{cases}
  \displaystyle \frac{\sin x}{x}, & x \neq 0 \\
  1, & x = 0
\end{cases}
\quad \text{与} \quad
A = \begin{pmatrix}
1 & 8 & 4 \\
7 & 9 & 2 \\
3 & 5 & 6
\end{pmatrix}
$$

字号与颜色支持：

$$
{\color{#3498db} \Huge \mathbb{N} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R} \subset \mathbb{C}}
$$
