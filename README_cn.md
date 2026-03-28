# Riskfolio-Lib

**Python中的投资组合优化，让每个人都变得简单。**

<a href="https://www.kqzyfj.com/click-101360347-15150084?url=https%3A%2F%2Flink.springer.com%2Fbook%2F9783031843037" target="_blank">
<div>
<img src="https://raw.githubusercontent.com/dcajasn/Riskfolio-Lib/refs/heads/master/docs/source/_static/Button.png" height="40" />
</div>
</a>
<a href="https://www.paypal.com/ncp/payment/GN55W4UQ7VAMN" target="_blank">
<div>
<img src="https://raw.githubusercontent.com/dcajasn/Riskfolio-Lib/refs/heads/master/docs/source/_static/Button2.png" height="40" />
</div>
<br>
</a>

<div class="row">
<img src="https://raw.githubusercontent.com/dcajasn/Riskfolio-Lib/master/docs/source/images/MSV_Frontier.png" height="200">
<img src="https://raw.githubusercontent.com/dcajasn/Riskfolio-Lib/master/docs/source/images/Pie_Chart.png" height="200">
</div>

[![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/dcajasn)

<a href='https://ko-fi.com/B0B833SXD' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://cdn.ko-fi.com/cdn/kofi1.png?v=2' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>

[![GitHub stars](https://img.shields.io/github/stars/dcajasn/Riskfolio-Lib)](https://github.com/dcajasn/Riskfolio-Lib/stargazers)
[![Downloads](https://static.pepy.tech/personalized-badge/riskfolio-lib?period=total&units=INTERNATIONAL_SYSTEM&left_color=GREY&right_color=BRIGHTGREEN&left_text=downloads)](https://pepy.tech/projects/riskfolio-lib)
[![Downloads per Month](https://static.pepy.tech/personalized-badge/riskfolio-lib?period=monthly&units=INTERNATIONAL_SYSTEM&left_color=GREY&right_color=ORANGE&left_text=downloads%2Fmonth)](https://pepy.tech/projects/riskfolio-lib)
[![Documentation Status](https://readthedocs.org/projects/riskfolio-lib/badge/?version=latest)](https://riskfolio-lib.readthedocs.io/en/latest/?badge=latest)
[![GitHub License](https://img.shields.io/github/license/dcajasn/Riskfolio-Lib)](https://github.com/dcajasn/Riskfolio-Lib/blob/master/LICENSE.txt)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dcajasn/Riskfolio-Lib/HEAD)

[![Star History Chart](https://api.star-history.com/svg?repos=dcajasn/Riskfolio-Lib&type=timeline&legend=top-left)](https://www.star-history.com/#dcajasn/Riskfolio-Lib&type=timeline&legend=top-left)

## 简介

Riskfolio-Lib 是一个用于进行 __Python 投资组合优化__ 的库，来自秘鲁 &#x1F1F5;&#x1F1EA;。它的目标是帮助学生、学者和从业人员以低成本基于复杂的数学模型建立投资组合。它构建于 [CVXPY](https://www.cvxpy.org/) 之上，并与 [Pandas](https://pandas.pydata.org/) 数据结构紧密集成。

Riskfolio-Lib 提供的一些关键功能：

- 具有 4 种目标函数的均值风险（Mean Risk）和对数均值风险（凯利准则）投资组合优化：

    - 最小化风险 (Minimum Risk)。
    - 最大化回报 (Maximum Return)。
    - 最大化效用函数 (Maximum Utility Function)。
    - 最大化风险调整后回报率 (Maximum Risk Adjusted Return Ratio)。

- 具有 24 种凸风险度量（convex risk measures）的均值风险和对数均值风险（凯利准则）投资组合优化：

    **离散风险度量 (Dispersion Risk Measures):**

    - 标准差 (Standard Deviation)。
    - 峰度平方根 (Square Root Kurtosis)。
    - 平均绝对偏差 (Mean Absolute Deviation, MAD)。
    - 基尼平均差 (Gini Mean Difference, GMD)。
    - 条件风险价值范围 (Conditional Value at Risk Range)。
    - 尾部基尼范围 (Tail Gini Range)。
    - 熵风险价值范围 (Entropic Value at Risk Range)。
    - 相对风险价值范围 (Relativistic Value at Risk Range)。
    - 极差 (Range)。
    &nbsp;

    **下行风险度量 (Downside Risk Measures):**

    - 半标准差 (Semi Standard Deviation)。
    - 半峰度平方根 (Square Root Semi Kurtosis)。
    - 一阶下偏矩（Omega 比率）。
    - 二阶下偏矩（Sortino 比率）。
    - 条件风险价值 (Conditional Value at Risk, CVaR)。
    - 尾部基尼 (Tail Gini)。
    - 熵风险价值 (Entropic Value at Risk, EVaR)。
    - 相对风险价值 (Relativistic Value at Risk, RLVaR)。
    - 最差实现（极小化极大，Minimax）。
    &nbsp;

    **回撤风险度量 (Drawdown Risk Measures):**

    - 非复利累计回报的平均回撤 (Average Drawdown)。
    - 非复利累计回报的溃疡指数 (Ulcer Index)。
    - 非复利累计回报的条件回撤风险 (Conditional Drawdown at Risk, CDaR)。
    - 非复利累计回报的熵回撤风险 (Entropic Drawdown at Risk, EDaR)。
    - 非复利累计回报的相对回撤风险 (Relativistic Drawdown at Risk, RLDaR)。
    - 非复利累计回报的最大回撤（Calmar 比率）。

- 具有 20 种凸风险度量的风险平价 (Risk Parity) 投资组合优化：

    **离散风险度量 (Dispersion Risk Measures):**

    - 标准差。
    - 峰度平方根。
    - 平均绝对偏差 (MAD)。
    - 基尼平均差 (GMD)。
    - 条件风险价值范围。
    - 尾部基尼范围。
    - 熵风险价值范围。
    - 相对风险价值范围。
    &nbsp;

    **下行风险度量 (Downside Risk Measures):**

    - 半标准差。
    - 半峰度平方根。
    - 一阶下偏矩（Omega 比率）。
    - 二阶下偏矩（Sortino 比率）。
    - 条件风险价值 (CVaR)。
    - 尾部基尼。
    - 熵风险价值 (EVaR)。
    - 相对风险价值 (RLVaR)。
    &nbsp;

    **回撤风险度量 (Drawdown Risk Measures):**

    - 非复利累计回报的溃疡指数 (Ulcer Index)。
    - 非复利累计回报的条件回撤风险 (CDaR)。
    - 非复利累计回报的熵回撤风险 (EDaR)。
    - 非复利累计回报的相对回撤风险 (RLDaR)。

- 层次聚类投资组合优化：使用朴素风险平价（naive risk parity）的层次风险平价 (Hierarchical Risk Parity, HRP) 和层次等风险贡献 (Hierarchical Equal Risk Contribution, HERC)，支持 35 种风险度量：

    **离散风险度量 (Dispersion Risk Measures):**

    - 标准差。
    - 方差 (Variance)。
    - 峰度平方根。
    - 平均绝对偏差 (MAD)。
    - 基尼平均差 (GMD)。
    - 风险价值范围 (Value at Risk Range)。
    - 条件风险价值范围。
    - 尾部基尼范围。
    - 熵风险价值范围。
    - 相对风险价值范围。
    - 极差 (Range)。
    &nbsp;

    **下行风险度量 (Downside Risk Measures):**

    - 半标准差。
    - 半峰度四次方根 (Fourth Root Semi Kurtosis)。
    - 一阶下偏矩（Omega 比率）。
    - 二阶下偏矩（Sortino 比率）。
    - 风险价值 (Value at Risk, VaR)。
    - 条件风险价值 (CVaR)。
    - 尾部基尼 (Tail Gini)。
    - 熵风险价值 (EVaR)。
    - 相对风险价值 (RLVaR)。
    - 最差实现（极小化极大，Minimax）。
    &nbsp;

    **回撤风险度量 (Drawdown Risk Measures):**

    - 复利和非复利累计回报的平均回撤。
    - 复利和非复利累计回报的溃疡指数。
    - 复利和非复利累计回报的回撤风险 (Drawdown at Risk, DaR)。
    - 复利和非复利累计回报的条件回撤风险 (CDaR)。
    - 复利和非复利累计回报的熵回撤风险 (EDaR)。
    - 复利和非复利累计回报的相对回撤风险 (RLDaR)。
    - 复利和非复利累计回报的最大回撤（Calmar 比率）。

- 嵌套聚类优化 (Nested Clustered Optimization, NCO)，支持四种目标函数及其对应的可用风险度量：

    - 最小化风险 (Minimum Risk)。
    - 最大化回报 (Maximum Return)。
    - 最大化效用函数 (Maximum Utility Function)。
    - 等风险贡献 (Equal Risk Contribution)。

- 最差均值方差 (Worst Case Mean Variance) 投资组合优化。
- 放宽风险平价 (Relaxed Risk Parity) 投资组合优化。
- 有序加权平均 (Ordered Weighted Averaging, OWA) 投资组合优化。
- 使用 Black Litterman 模型的投资组合优化。
- 使用风险因子 (Risk Factors) 模型的投资组合优化。
- 使用 Black Litterman 贝叶斯 (Bayesian) 模型的投资组合优化。
- 使用增强型 (Augmented) Black Litterman 模型的投资组合优化。
- 具有跟踪误差 (tracking error) 和换手率 (turnover) 约束的投资组合优化。
- 具有空头头寸和杠杆的投资组合优化。
- 具有最大资产数量和有效资产数量约束的投资组合优化。
- 基于图信息 (graph information) 约束的投资组合优化。
- 具有方差风险贡献不等式约束的投资组合优化。
- 具有方差的因子风险贡献不等式约束的投资组合优化。
- 具有整数约束的投资组合优化，例如资产和类别的基数约束 (Cardinality)、互斥 (Mutually Exclusive) 和联合投资 (Join Investment)。
- 为 24 种凸风险度量构建有效边界的工具。
- 为资产、资产类别和风险因子构建线性约束的工具。
- 构建资产和资产类别观点的工具。
- 构建风险因子观点的工具。
- 构建每个资产类别的风险贡献约束的工具。
- 使用显式风险因子和主成分构建每个风险因子的风险贡献约束的工具。
- 为层次聚类投资组合构建边界约束的工具。
- 计算风险度量的工具。
- 计算每个资产的风险贡献的工具。
- 计算每个风险因子的风险贡献的工具。
- 计算均值向量和协方差矩阵不确定性集合的工具。
- 基于共依附指标 (codependence metrics) 计算资产聚类的工具。
- 估计载荷矩阵 (loadings matrix)（逐步回归和主成分回归）的工具。
- 可视化投资组合属性和风险度量的工具。
- 在 Jupyter Notebook 和 Excel 上构建报告的工具。
- 可选择使用商业优化求解器（如 MOSEK 或 GUROBI）处理大规模问题。


## 文档

在线文档可在 [Documentation](https://riskfolio-lib.readthedocs.io/en/latest/) 获取。

该文档包含一个[教程](https://riskfolio-lib.readthedocs.io/en/latest/examples.html)，通过示例展示了 Riskfolio-Lib 的功能。


## 选择求解器

由于 Riskfolio-Lib 基于 CVXPY，因此 Riskfolio-Lib 可以使用适用于 CVXPY 的相同求解器。兼容 CVXPY 的求解器列表可参见 CVXPY 文档的 [Choosing a solver](https://www.cvxpy.org/tutorial/advanced/index.html#choosing-a-solver) 部分。但是，为了给每个风险度量选择合适的求解器，我们可以参考下表，该表指明了用于建立每种风险度量模型的规划技术类型。

| 风险度量 (Risk Measure)               | LP | QP | SOCP | SDP | EXP | POW |
|---------------------------------------|----|----|------|-----|-----|-----|
| 方差 (Variance, MV)                   |    |    | X    | X*  |     |     |
| 平均绝对偏差 (MAD)                    | X  |    |      |     |     |     |
| 基尼平均差 (GMD)                      |    |    |      |     |     | X** |
| 半方差 (Semi Variance, MSV)           |    |    | X    |     |     |     |
| 峰度 (Kurtosis, KT)                   |    |    |      | X   |     |     |
| 半峰度 (Semi Kurtosis, SKT)           |    |    |      | X   |     |     |
| 一阶下偏矩 (FLPM)                     | X  |    |      |     |     |     |
| 二阶下偏矩 (SLPM)                     |    |    | X    |     |     |     |
| 条件风险价值 (CVaR)                   | X  |    |      |     |     |     |
| 尾部基尼 (Tail Gini, TG)              |    |    |      |     |     | X** |
| 熵风险价值 (EVaR)                     |    |    |      |     | X** |     |
| 相对风险价值 (RLVaR)                  |    |    |      |     |     | X** |
| 最差实现 (Worst Realization, WR)      | X  |    |      |     |     |     |
| CVaR 范围 (CVaR Range, CVRG)          | X  |    |      |     |     |     |
| 尾部基尼范围 (Tail Gini Range, TGRG)  |    |    |      |     |     | X** |
| EVaR 范围 (EVaR Range, EVRG)          |    |    |      |     | X** |     |
| RLVaR 范围 (RLVaR Range, RVRG)        |    |    |      |     |     | X** |
| 极差 (Range, RG)                      | X  |    |      |     |     |     |
| 平均回撤 (Average Drawdown, ADD)      | X  |    |      |     |     |     |
| 溃疡指数 (Ulcer Index, UCI)           |    |    | X    |     |     |     |
| 条件回撤风险 (CDaR)                   | X  |    |      |     |     |     |
| 熵回撤风险 (EDaR)                     |    |    |      |     | X** |     |
| 相对回撤风险 (RLDaR)                  |    |    |      |     |     | X** |
| 最大回撤 (Maximum Drawdown, MDD)      | X  |    |      |     |     |     |

(*) 当包含 SDP 图论约束或风险贡献约束时。如果包含整数规划图论约束，模型将假定采用 SOCP 形式。

(**) 对于这些模型，强烈推荐使用 MOSEK 作为求解器，因为在某些情况下，CLARABEL 无法找到解，而 SCS 则需要耗费过多的时间来求解。

LP - 线性规划 (Linear Programming)：指目标函数和约束条件均为线性的问题。

QP - 二次规划 (Quadratic Programming)：指具有二次目标函数和线性约束的问题。

SOCP - 二阶锥规划 (Second Order Cone Programming)：指具有二阶锥约束的问题。

SDP - 半正定规划 (Semidefinite Programming)：指具有半正定约束的问题。

EXP - 指具有指数锥约束的问题。

POW - 指具有 3 维幂锥约束的问题。


## 依赖项

Riskfolio-Lib 支持 Python 3.9 或更高版本。

安装需要：
- [numpy](http://www.numpy.org/) >= 1.26.0
- [scipy](https://www.scipy.org/) >= 1.13.0
- [pandas](https://pandas.pydata.org/) >= 2.2.2
- [matplotlib](https://matplotlib.org/) >= 3.9.2
- [clarabel](https://oxfordcontrol.github.io/ClarabelDocs/stable/) >= 0.11.1
- [scs](https://www.cvxgrp.org/scs/) >= 3.2.7
- [cvxpy](https://www.cvxpy.org/) >= 1.7.2
- [scikit-learn](https://scikit-learn.org/stable/) >= 1.7.0
- [statsmodels](https://www.statsmodels.org/) >= 0.14.5
- [arch](https://bashtage.github.io/arch/) >= 7.2
- [xlsxwriter](https://xlsxwriter.readthedocs.io) >= 3.2.2
- [networkx](https://networkx.org) >= 3.4.2
- [astropy](https://www.astropy.org) >= 6.1.3
- [pybind11](https://pybind11.readthedocs.io/en/stable/) >= 2.13.6
- [vectorbt](https://vectorbt.dev) >= 0.28.0


## 安装

可以从 PyPI 安装最新的稳定版本（以及旧版本）：

    pip install riskfolio-lib


## 引用

如果您将 Riskfolio-Lib 用于已发表的作品，请使用以下 BibTeX 条目：

```
@misc{riskfolio,
      author = {Dany Cajas},
      title = {Riskfolio-Lib (7.2.1)},
      year  = {2026},
      url   = {https://github.com/dcajasn/Riskfolio-Lib},
      }
```

## 开发

Riskfolio-Lib 的开发在 Github 上进行：https://github.com/dcajasn/Riskfolio-Lib


## 咨询费用

Riskfolio-Lib 是一个开源项目，但由于它是一个没有接受任何机构资助的项目，因此我开始对与源代码错误无关的咨询收费。我们的收费标准如下：

- 每提出一个不需要检查代码的问题，收费 $ 25 USD（美元）。
- 检查小型脚本或代码（少于 200 行代码）收费 $ 50 USD。解决方案的费用取决于解决方案的复杂性：
    - 脚本中的简单错误（修改少于 10 行代码）收费 $ 50 USD。
    - 对于绝大多数复杂错误，费用取决于解决方案的复杂性，费率为每小时 $ 150 USD。
- 检查中型脚本或代码（201 至 600 行代码）收费 $ 100 USD。解决方案的费用取决于解决方案的复杂性：
    - 脚本中的简单错误（修改少于 10 行代码）收费 $ 50 USD。
    - 对于绝大多数复杂错误，费用取决于解决方案的复杂性，费率为每小时 $ 150 USD。
- 对于大型脚本或代码（超过 600 行代码），费用根据代码的规模而定。解决方案的费用取决于解决方案的复杂性：
    - 脚本中的简单错误（修改少于 10 行代码）收费 $ 50 USD。
    - 对于绝大多数复杂错误，费用取决于解决方案的复杂性，费率为每小时 $ 150 USD。

**所有咨询费用必须预先支付**。

您可以通过以下方式联系我：

- __[LinkedIn](https://www.linkedin.com/in/dany-cajas/)__
- __[Gmail](dcajasn@gmail.com)__

您可以使用以下渠道之一进行付款：

- __[Github Sponsorship](https://github.com/sponsors/dcajasn)__

- <a href='https://ko-fi.com/B0B833SXD' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://cdn.ko-fi.com/cdn/kofi1.png?v=2' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>

## 路线图 (RoadMap)

此模块的计划是添加对资产管理者非常实用的更多函数。

- 根据用户建议添加更多功能。
