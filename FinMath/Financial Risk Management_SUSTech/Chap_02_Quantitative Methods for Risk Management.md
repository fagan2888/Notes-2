# Quantitative Methods for Risk Management

$$
% bbox
% \bbox[#EEF, 5px, border: 2px solid #880015]{E=mc^2}
% \bbox[9px, border:2px solid #880015]{abc}
% text size
% tiny scriptsize small normalsize large Large LARGE huge Huge
% color
% aquamarine, black, blue, brown, cyan, darkgray, gray, green, lightgray, lime, magenta, olive, orange, pink, purple, red, teal, violet, white, yellow
\DeclareMathOperator*{\argmin}{argmin}
\DeclareMathOperator*{\argmax}{argmax}
\DeclareMathOperator*{\plim}{plim}
\DeclareMathOperator*{\span}{span}
\newcommand{\space}{\;\;}
\newcommand{\bspace}{\;\;\;}
\newcommand{\Bspace}{\;\;\;\;}
\newcommand{\bbspace}{\;\;\;\;\;}
\newcommand{\BBspace}{\;\;\;\;\;\;}
\newcommand{\QQQ}{\boxed{?\:}}
\newcommand{\void}{\left.\right.}
% \newcommand{\myEmphy}[2][#880015]{\color{#1}{#2}}
% \newcommand{\myEmphyQ}{\color{#880015}}
% \newcommand{\myBox}[2][9px, border:2px solid #880015]{\bbox[#1]{#2}}
% \newcommand{\myBoxQ}{\bbox[9px, border:2px solid #880015]}
\newcommand{\myEmphy}[2][#880015]{ {\color{#1}{#2}} }
\newcommand{\myBox}[2][9px, border:2px solid #880015]{ {\bbox[#1]{#2}} }
\newcommand{\d}[1]{ {\displaystyle{#1}} }
\newcommand{\Tran}[1]{{#1}^{\mathrm{T}}}
\newcommand{\CB}[1]{\left\{ #1 \right\}}
\newcommand{\SB}[1]{\left[ #1 \right]}
\newcommand{\Pare}[1]{\left( #1 \right)}
\newcommand{\abs}[1]{\left| #1 \right|}
\newcommand{\norm}[1]{\left\| #1 \right\|}
\newcommand{\given}[1]{\left. #1 \right|}
\newcommand{\using}[2][=]{\overset{\mathrm{#2}}{#1}}
\newcommand{\usingUD}[3][=]{\underset{\text{#2}}{\overset{\text{#3}}{#1}}}
\newcommand{\tinyText}[1]{ {\tiny{\text{#1}}} }
\newcommand{\scriptsizeText}[1]{ {\scriptsize{\text{#1}}} }
\newcommand{\footnotesizeText}[1]{ {\footnotesize{\text{#1}}} }
\newcommand{\smallText}[1]{ {\small{\text{#1}}} }
\newcommand{\largeText}[1]{ {\large{\text{#1}}} }
\newcommand{\LargeText}[1]{ {\Large{\text{#1}}} }
\newcommand{\LARGEText}[1]{ {\LARGE{\text{#1}}} }
\newcommand{\hugeText}[1]{ {\huge{\text{#1}}} }
\newcommand{\HugeText}[1]{ {\Huge{\text{#1}}} }
\newcommand{\RR}{\mathbb{R}}
\newcommand{\EE}{\mathbb{E}}
\newcommand{\FF}{\mathbb{F}}
\newcommand{\II}{\mathbb{I}}
\newcommand{\NN}{\mathbb{N}}
\newcommand{\ZZ}{\mathbb{Z}}
\newcommand{\QQ}{\mathbb{Q}}
\newcommand{\PP}{\mathbb{P}}
\newcommand{\AcA}{\mathcal{A}}
\newcommand{\CcC}{\mathcal{C}}
\newcommand{\FcF}{\mathcal{F}}
\newcommand{\IcI}{\mathcal{I}}
\newcommand{\NcN}{\mathcal{N}}
\newcommand{\AsA}{\mathscr{A}}
\newcommand{\FsF}{\mathscr{F}}
\newcommand{\IsI}{\mathscr{I}}
\newcommand{\dd}{\mathrm{d}}
\newcommand{\asim}{\overset{\text{a}}{\sim}}
\newcommand{\idctV}{\mathbf{1}}
\newcommand{\refs}[1]{ \tag{#1}\label{#1} }
\newcommand{\I}[1]{\mathrm{I}\left( #1 \right)}
\newcommand{\N}[1]{\mathcal{N}\left( #1 \right)}
\newcommand{\Exp}[1]{\mathrm{E}\left[ #1 \right]}
\newcommand{\Var}[1]{\mathrm{Var}\left[ #1 \right]}
\newcommand{\Avar}[1]{\mathrm{Avar}\left[ #1 \right]}
\newcommand{\Cov}[1]{\mathrm{Cov}\left( #1 \right)}
\newcommand{\Corr}[1]{\mathrm{Corr}\left( #1 \right)}
\newcommand{\ExpH}{\mathrm{E}}
\newcommand{\VarH}{\mathrm{Var}}
\newcommand{\AVarH}{\mathrm{Avar}}
\newcommand{\CovH}{\mathrm{Cov}}
\newcommand{\CorrH}{\mathrm{Corr}}
\newcommand{\ow}{\text{otherwise}}
\newcommand{\wp}{\text{with probability }}
\newcommand{\VaR}{\text{VaR}}
\newcommand{\FSD}{\text{FSD}}
\newcommand{\SSD}{\text{SSD}}
\newcommand{\QED}{\myEmphy{\blacksquare}}
\newcommand{\SUM}{\myEmphy{\text{Summary}}}
\newcommand{\pf}{\myEmphy{\largeText{Proof}}}
\newcommand{\slu}{\myEmphy{\largeText{Solution}}}
\newcommand{\Corlr}{\myEmphy{\largeText{Corrollary}}}
\newcommand{\Rmk}{\myEmphy{\largeText{Remark}}}
\newcommand{\pops}[1]{\myEmphy{\largeText{Proposition #1}}}
\newcommand{\Pops}{\myEmphy{\largeText{Proposition}}}
\newcommand{\zrm}[1]{\myEmphy{\largeText{Theorem #1}}}
\newcommand{\Zrm}{\myEmphy{\largeText{Theorem}}}
\newcommand{\ppt}[1]{\myEmphy{\largeText{Property #1}}}
\newcommand{\Ppt}{\myEmphy{\largeText{Property}}}
\newcommand{\def}[1]{\myEmphy{\largeText{Definition #1}}}
\newcommand{\Def}{\myEmphy{\largeText{Definition}}}
\newcommand{\lm}[1]{\myEmphy{\largeText{Lemma #1}}}
\newcommand{\Lm}{\myEmphy{\largeText{Lemma}}}
\newcommand{\eg}[1]{\myEmphy{\largeText{Example #1}}}
\newcommand{\ex}[1]{\myEmphy{\largeText{Exercise.#1}}}
\newcommand{\rmk}[1]{\myEmphy{\largeText{Remark #1}}}
\myEmphy{\smallText{Xavier}}
$$



## Types of ﬁnancial risks and loss distributions

$\Def$ Risk

- loss or exposure to mischance
- volatility of unexpected outcomes

**Risk management** is the process by which various risk exposures are identiﬁed, measured, and controlled.



### Market risk

due to the volatility of market price

- Absolute risk, measured in dollar terms
- Relative risk, measured relative to a benchmark index



$\Def$ Directional risk

 due to the direction of movements in ﬁnancial variables

- **Duration**, with interest rate
- **Delta**, with underlying asset price

$\Def$ Non-directional risks

due to Non-linear exposures and exposures to hedged positions or to volatilities

- **Convexity**, with interest rate
- **Gamma**, with underlying asset price
- **Volatility risk**, due to actual or implied volatility
- **Basis risk**: when offsetting investments in a hedging strategy do not experience price changes in entirely opposite directions from each other. For example: The *imperfect correlation* between the two investments creates the potential for excess gains or losses in a hedging strategy



### Credit risk

- quantiﬁed by the (yield) spread, which is the yield above the risk-free Treasury rate (while higher risk, higher YTM, lower bond price)

$\Def$ **Default risk**

any non-compliance with the exact speciﬁcation of a contract

- **Arrival risk**: timing of the event, modeled by a stopping time $\tau$
- **Magnitude risk**: $\text{loss amount}=\text{par value}-\text{market value of a defaultable bond}$
  - loss amount: exposure net of the recovery value
  - par value possibly with accrued interest

$\Def$ **Spread risk**

reduction in market value of the contract / instrument due to changes in the **credit quality** of the debtor / counterparty

with elements

- exposure at default, $r.v.$

- recovery rate, $r.v.$

- default probability

  - default criteria

  - time of default, $r.v.$ 

- **Credit migration**: the process of changing the creditworthiness of an obligor as characterized by the transition probabilities from one credit state to other credit states

  - Occurs when the calculation agent is aware of publicly available information as to the existence of a credit condition
  - **Credit condition**: either a payment default or a bankruptcy event in respect of the issuer
  - **Publicly available information**: information that has been published in any two or more internationally recognized published or electronically displayed ﬁnancial news sources
  - drivers
    - future earnings and cash-ﬂow
    - debts, short-term and long-term liabilities, and ﬁnancial obligations
    - capital structure (leverage)
    - liquidity of the ﬁrm’s assets
    - political situations
    - industrial situations
    - management quality, company structure, etc



### Liquidity risk

due to lack of marketability, that cannot be bought or sold quickly enough to prevent or minimize a loss

and this risk occurs when investor cannot meet short-term debt obligations

measured by bid-offer spread: $\text{spred/bid}\downarrow \implies $ risk$\;\uparrow$



### Operational risk

due to human and technical errors or accidents

- **Fraud**, management failure, and inadequate procedures and controls
- Back-office operations that record transactions
- **Model risk**: flawed mathematical model to value position



###  Legal risk

due to transaction proved unenforceable in law

Legal risk is generally related to credit risk



### Business risk

risk arising from strategic decisions or reputational risk

Regulatory capital is not required for business risk under Basel II.



$\eg{}$ bank

<img src="assets/1550640843100.png" width=400>



$\eg{}$ Long Term Capital Management

LTCM is a hedge fund formed in the mid 1990s. The hedge fund's investment strategy was known as **convergence arbitrage**:

- bonds: $X$, $Y$, from same company, with same payoff
- liquidity: $X<Y \implies$ price: $X < Y$
- buy $X$, short $Y$
- time pass and expected price of $X$, $Y$ converge $\implies$ profit

<u>Advantage</u>: no signiﬁcant outﬂow from its collateralization agreements, as $i \uparrow$ or $\downarrow$

$i\uparrow \implies$ price $X,Y\downarrow$, with similar amount $\implies$

collateral paid on $X\approx$ collateral received from $Y$

<u>Death</u>: August 1998

Russia defaulted $\implies$ "*flight to quality*" in capital markets $\implies$

investors valued liquid instruments more $\implies$

$X$ less liquidity $\implies$ price $X \downarrow\implies$ pay collateral 

$Y$ more liquidity $\implies$ price $Y \uparrow\implies$ pay collateral

LTCM is highly leveraged $\implies$ position closed $\implies$ Death

$\eg{}$ European Growth Trust

1. Peter Young managed this fund with over $£ 1$ billion
2. P. Young violated a rule, and benefited himself
3. facts were uncovered, he was ﬁred, his employer compensate over $£ 200$ million



### Capital reserve

- meet regulatory requirements
- act as a buﬀer during ﬁnancial hardship
- by charging an appropriate **risk premium** for every **loan**

$\Def$ Loss variable
$$
\tilde L = \text{EAD}\times\text{SEV}\times L
$$

- exposure at default: $\text{EAD}$
- severity: $\text{SEV}\implies$loss given default: $\text{LGD}=\Exp{\text{SEV}} =1-\text{recovery rate}$
- default event $D\implies L=\mathbf{1}_D\implies$ default probability: $\text{DP}=\Exp{L}$
- Assumption
  - exposure, severity and default event are independent
  - $\text{EAD}$ is deterministic, could be the expectation of some underlying $r.v.$

$\implies$ the expected loss
$$
\myBox{\text{EL}=\Exp{\tilde L} = \text{EAD}\times \text{LGD}\times\text{DP}}
$$
$\Def$ Unexpected loss

standard deviation: $\text{UL}=\sqrt{\Var{\tilde L}}$, under assumption:
$$
\myBox{\text{UL}=\text{EAD}\times\sqrt{\Var{\text{SEV}} \times \text{DP}+\text{LGD}^2\times \text{DP}\Pare{1-\text{DP}}}}
$$
$\pf$
$$
\begin{align}
\text{UL}^2 &={\Var{\tilde L}} = \Exp{\tilde L^2}-\text{EL}^2\\
& = \text{EAD}^2\times\Exp{\text{SEV}^2}\times\Exp{\mathbf{1}_D^2} -\text{EAD}^2\times \text{LGD}^2\times\text{DP}^2 \\
& =\text{EAD}^2\Pare{ \Pare{\Exp{\text{SEV}^2}-\text{LGD}^2}\text{DP}+ \Pare{\text{LGD}^2\cdot\text{DP}-\text{LGD}^2\times\text{DP}^2}}\\
& =\text{EAD}^2\Pare{{\Var{\text{SEV}} \times \text{DP}+\text{LGD}^2\times \text{DP}\Pare{1-\text{DP}}}}
\end{align}
$$
$\QED$

$\Rmk$

- $\Exp{\mathbf{1}^2_D}=\Exp{\mathbf{1}_D}=\text{DP}$
- actually $\text{SEV}$ and $\mathbf1_D$ may be not independent 



$\Def$ Portfolio loss

$m$ loans
$$
\myEmphy{\tilde L_p = \sum_{i=1}^m \tilde L_i = \sum \text{EAD}_i\times\text{SEV}_i\times\mathbf{1}_{D_i}}\\
\implies \myBox{\Exp{\tilde L_p}= \sum_{i=1}^m \Exp{\tilde L_i} = \sum \text{EAD}_i\times\text{LGD}_i\times\text{DP}_i }\\
\implies \myBox{\text{UL}_p = \sqrt{\sum_{i=1}^m\sum_{j=1}^m \text{EAD}_i\times \text{EAD}_j\times\Cov{\text{SEV}_i\times\mathbf{1}_{D_i},\text{SEV}_j\times\mathbf{1}_{D_j}}  }}
$$
if constant severities $\text{SEV} \implies \text{LGD}=\text{SEV}\implies$
$$
\myBox{\text{UL}_p^2 = \sum_{i=1}^m\sum_{j=1}^m \text{EAD}_i\times \text{EAD}_j\times\text{LGD}_i\times\text{LGD}_j\times\sqrt{\text{DP}_i\Pare{1-\text{DP}_i}}\times\sqrt{\text{DP}_j\Pare{1-\text{DP}_j}}\times\rho_{ij}}
$$
Here $\rho_{ij}$ is the correlation coefficient between default events
$$
\rho_{ij} = \frac{\Cov{\mathbf{1}_{D_i},\mathbf{1}_{D_j}}}{\sqrt{\Var{\mathbf{1}_{D_i}}\Var{\mathbf{1}_{D_j}}}}
$$


$\Corlr$ 
$$
\myBox{\frac{\partial \text{UL}_p}{\partial \text{UL}_i} = \frac{\sum_{j=1}^m \text{UL}_j \rho_{ij}}{\text{UL}_p}}
$$
$\pf$
$$
\begin{align}
\myEmphy{\text{UL}_p^2} &= \Var{\sum_{i=1}^m \tilde L_i} = \sum_{i=1}^m\sum_{j=1}^m \Cov{\tilde L_i,\tilde L_j}=\myBox{\myEmphy{\sum_{i=1}^m\sum_{j=1}^m \text{UL}_i\text{UL}_j\rho_{ij}}}\\
\implies \myEmphy{\frac{\partial \text{UL}_p^2}{\partial \text{UL}_i}} & = \myEmphy{2\sum_{j=1}^m \text{UL}_j \rho_{ij}}\\
\end{align}
$$
At the same time, 
$$
\frac{\partial \text{UL}_p^2}{\partial \text{UL}_i} = 2\text{UL}_p\cdot \frac{\partial \text{UL}_p}{\partial \text{UL}_i}
$$
$\QED$



$\Def$ <span id = "Risk-contribution">Risk contribution<span>

$i$: risky asset

$\text{UL}_p$: portfolio unexpected loss

$\implies $ incremental risk
$$
\myBox{\text{RC}_i = \text{UL}_i\frac{\partial\text{UL}_p}{\partial \text{UL}_i} = \frac{\text{UL}_i}{\text{UL}_p}\cdot\sum_{j=1}^m \text{UL}_j \rho_{ij}  }
$$
$\Corlr$
$$
\myBox{\text{UL}_p=\sum_i \text{RC}_i}
$$
$\pf$
$$
\begin{align}
\sum_i \text{RC}_i& = \sum_i\Pare{\frac{\text{UL}_i}{\text{UL}_p}\cdot\sum_{j=1}^m \text{UL}_j \rho_{ij}}\\
&= \frac{\sum_{i=1}^m\text{UL}_i\sum_{j=1}^m \text{UL}_j \rho_{ij}}{\text{UL}_p}\\
&= \frac{\sum_i\sum_j\text{UL}_i \text{UL}_j \rho_{ij}}{\text{UL}_p}\\
&= \frac{\text{UL}_p^2}{\text{UL}_p} = \text{UL}_p
\end{align}
$$
$\QED$



$\eg{}$ two-asset portfolio

- individual expected loss: $\myEmphy{\text{EL}_i=\Exp{\tilde L_i} = \Exp{\text{EAD}_i\times\text{SEV}_i\times \mathbf{1}_{D_i}}=\text{EAD}_i\times \text{LGD}_i\times\text{DP}_i}$
- portfolio expected loss: ${\myEmphy{\text{EL}_p=\text{EL}_1+\text{EL}_2}}$
- correlation: ${\myEmphy{\rho_{12} = \dfrac{\Cov{\mathbf{1}_{D_1},\mathbf{1}_{D_2}}}{\sqrt{\Var{\mathbf{1}_{D_1}}\Var{\mathbf{1}_{D_2}}}}}}$
- individual unexpected loss: ${\myEmphy{\text{UL}_i= \text{EAD}_i \times \sqrt{\Var{\text{SEV}_i} \times \text{DP}_i+\text{LGD}_i^2\times \text{DP}_i\Pare{1-\text{DP}_i}}}}$
- risk contribution from Exposure 1: $\myEmphy{\text{RC}_1=\text{UL}_1\Pare{\text{UL}_1+\rho \text{UL}_2}/\text{UL}_p}$
- risk contribution from Exposure 2: $\myEmphy{\text{RC}_2=\text{UL}_2\Pare{\text{UL}_2+\rho \text{UL}_1}/\text{UL}_p}$
- portfolio unexpected loss: $\myEmphy{{\text{UL}_p=\sqrt{\text{UL}_1^2+\text{UL}_2^2+2\rho \text{UL}_1\text{UL}_2}}=\text{RC}_1+\text{RC}_2}$



$\Def$ Skewness

the departure from symmetry
$$
\gamma = \frac{\Exp{\Pare{x-\Exp{X}}^3}}{\sigma^3} = \frac{\int_{-\infty}^\infty{\Pare{x-\Exp{X}}^3}f\Pare{x}\,\dd x}{\sigma^3}
$$

- normal distribution: $\gamma=0$
- $\gamma>0\implies$ long right tail $\implies$ entails large positive value

$\Def$ Kurtosis

the degree of flatness of a distribution
$$
\kappa = \frac{\Exp{\Pare{x-\Exp{X}}^4}}{\sigma^4} = \frac{\d{\int_{-\infty}^\infty{\Pare{x-\Exp{X}}^4}f\Pare{x}\,\dd x}}{\sigma^4}
$$

- normal distribution: $\kappa=3$
- $\kappa>3\implies$ the tails (right and left) decay less quickly $\implies$ a greater likelihood of large value in both tails



### Monte Carlo simulation of loss

Let

- $n$: time of simulation
- ${\tilde L_p^{\Pare{j}}}$: portfolio loss in $j$th simulation
- ${\idctV_{\SB{0,x}}\Pare{y}=\begin{cases}1&y\leq x\\ 0& y>x\end{cases} \implies}$ Bernoulli variable $\idctV_{\SB{0,x}}\Pare{\tilde L_p^{\Pare{n}}}$

**empirical loss distribution function**:
$$
\myBox{F\Pare{x} = \frac{1}{n}\sum_i  \idctV_{\SB{0,x}}\Pare{\tilde L_p^{\Pare{i}}} }
$$
the proportion of random ${\tilde L_p^{\Pare{j}}}$ out of $n$ when it falls within $\SB{0,x}$



### Fitting of loss distribution

$\Def$ **model risk**

due to using the quantiles of the approximating $r.v.$ $X$ to model the original portfolio



$\Zrm$ **beta distribution**

Let
$$
\myBox{\Gamma\Pare\alpha = \int_0^\infty e^{-x}x^{\alpha-1}\;\dd x,\BBspace\Gamma\Pare\beta = \int_0^\infty e^{-x}x^{\beta-1}\;\dd x}
$$
here $\alpha,\beta>0 \implies$
$$
\myBox{
f\Pare{x,\alpha,\beta} =\begin{cases}
\d{ \frac{\Gamma\Pare{\alpha+\beta}}{\Gamma\Pare\alpha\Gamma\Pare\beta} x^{\alpha-1}\Pare{1-x}^{\beta-1}  }, & 0<x<1\\[1em]
0,&\ow
\end{cases}
}
$$
$\implies$
$$
\myBox{\mu = \frac{\alpha}{\alpha+\beta},\BBspace\sigma^2=\frac{\alpha\beta}{\Pare{\alpha+\beta}^2\Pare{\alpha+\beta+1}}}
$$
<img src="assets/1550677467232.png" width=400>



$\slu$ steps
$$
\myEmphy{\tilde L_p = \sum_{i=1}^m \tilde L_i = \sum \text{EAD}_i\times\text{SEV}_i\times\mathbf{1}_{D_i}}
$$
by matching the *first and second moments* of the portfolio loss distribution

- mean: portfolio expected loss
- standard deviation: portfolio unexpected loss

#### Step 1: Estimate default and losses

1. use risk ratings to loss facilities and determine their **default probability**: $\text{DP}=\Exp{\mathbf{1}_D}=\Exp{\mathbf{1}^2_D}$
2. find or just assign the $\text{LGD} = \Exp{\text{SEV}}$, 
3. find or just assign the $\sigma_{\text{LGD}} = \Var{\text{SEV}}$

#### Step 2: Estimate asset correlation between obligors

1. determine pairwise asset correlation
2. (if there is) determine industry pair correlation

#### Step 3: Generate random loss given default

The $\text{SEV}$ is a stochastic variable with unknown distribution.

$\eg{}$
$$
\begin{array}{cccc}\hline
 &\text{Recovery rate (%)} & \text{LGD(%)} & \sigma_{\text{LGD}}\text{(%)}\\\hline
 \text{secured} & 65 & 35 & 21\\
 \text{unsecured} & 50 & 50 & 28\\\hline
\end{array}
$$

$$
\text{SEV}_i=\text{LGD}_i^s+f_i\times\sigma_{\text{LGD},i}^s
$$

$f_i$: drawn from a uniform distribution, such that $\text{SEV}$ has a standard deviation that is consistent with historical observation ([Step 1](#Step-2:-Estimate-asset-correlation-between-obligors))

#### Step 4: Generate correlated default events

##### Decomposition of a covariance matrix

1. Generate a set of random numbers drawn from a **standard normal distribution**: $\vec{v}$
2. decompose (Cholesky, SVD, or eigenvalue) the asset correlation matrix$\implies \vec{w}$, a set of correlated asset values
3. Find matrix $M$, such that
   - $\Tran{M}M=\Sigma$, covariance matrix
   - $\vec w=M\vec v$, transformation matrix

##### Calculation of the default point

Assume: credit indexes follow standard normal distribution

1. **default probability** $\text{DP}$ $\implies$ **default point threshold** $\text{DT}_i$: $\text{DP}=\N{\text{DT}_i}$
2. for obligor $i$: $\begin{cases}\text{default},&\text{if } \vec w_i < \text{DT}_i\\[0.7em] \text{not default},&\text{if } \vec w_i \geq \text{DT}_i\end{cases}$

#### Step 5: Loss calculation

$$
\text{Loss}=\sum_{\text{Obligors in default}} \text{Adjusted exposure}_i\times \text{SEV}_i
$$

#### Step 6: Simulate loss distribution

just repeat the previous steps sufficiently



$\Rmk$ As for the default risk

- substantial variability
- generally low correlation
- dynamic and subject to large fluctuation
- can be effectively managed through **diversiﬁcation**
  - lower loss than expected
  - huge loss infrequently

$\Rmk$ Distribution for loss density function

|                         market risk                          |                         credit risk                          |                       operational risk                       |
| :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| <img src="D:\Notes\FinMath\Financial Risk Management_SUSTech\assets\1552146672007.png" width=200> | <img src="D:\Notes\FinMath\Financial Risk Management_SUSTech\assets\1552146698528.png" width=200> | <img src="D:\Notes\FinMath\Financial Risk Management_SUSTech\assets\1552146702661.png" width=200> |
|                       $t$-distribution                       |                            skewed                            |                        extreme shape                         |

<img src="D:\Notes\FinMath\Financial Risk Management_SUSTech\assets\1552146879860.png" width=400>



## VaR, expected shortfall and coherent risk measure

### VaR

$\Def$ Value at risk

> I am $X$ percent certain, that there will *NOT* be a loss of *more* than $V$ dollars in the next $N$ days.
>
> How bad can things get? Give me one number

$N$: time horizon

$X\%$: confidence level

$\implies \VaR$: the loss level over $N$ days that has a probability of only $\Pare{100-X}\%$ of being exceeded

or

$\VaR$, the loss corresponding to the $\Pare{100-X}$th percentile of the distribution of the *change in the value of the portfolio* over the next $N$ days

or

$\VaR$, is the $X$th **percentile** of the distribution of *loss*
$$
\myBox{
\begin{align}
\VaR_X\Pare{\tilde L} &= \inf\CB{I\in\RR,P\Pare{\tilde L>I}\leq 1-X}\\
&= \inf\CB{I\in\RR,P\Pare{\tilde L\leq I}\geq X}\\
\implies P\Pare{\tilde L \leq \VaR_X\Pare{\tilde L}}&=X
\end{align}}
$$


<img src="assets/1550738645542.png" width=400>

$\Rmk$

$\VaR$ is the corresponding value in horizontal axis when the cdf reaches $X$ percent, in the distribution graph.

so even when $\VaR$ is the same, potential loss may be not, and severe loss maybe more likely to happen

<img src="assets/1550736707364.png" width=400>



$\Rmk$

In real world, $\tilde L\geq \text{EL}+\text{UL}$, since there might be a significant likelihood that losses will exceed $\text{EL}$ by one standard deviation ($\mu+\sigma$)



$\eg{}$

Suppose

$T$: $6$ months

gain: normal $r.v.$

- mean: $\$2$ million
- standard deviation: $\$10$ million

$\slu$

$X=99$

standard cdf: $\myEmphy{\d{\N{x}=\int_{-\infty}^x\frac{1}{\sqrt{2\pi}} e^{-t^2/2}\;\dd t  }}$

$\implies$ one percentile point: $\mu-\sigma\cdot z=2-2.33\times  10 = -21.3$ million

$\implies$ $\VaR$ for the portfolio with a time horizon of six months and confidence level of $99\%$ is $21.3$ million

$\eg{}$

Suppose

$T$: 1 year

- $98\%$ chance gain of $\$2$ million
- $1.5\%$ chance loss $\$4$ million
- $0.5\%$ chance loss $\$10$ million

$\slu$

Draw its cdf

<img src="assets/1550741301058.png" width=400>

$X=99\implies \VaR=\$4$ million

$X=99.5\implies\myBox{\VaR=\dfrac{\$4+\$10}{2}}=\$7$ million

$\Rmk$

we see that $\VaR$ is *NOT* uniquely defined, thus we would choose its **midpoint** of the range of possible $\VaR$ value



### Expected Shortfall

$\Def$ tail conditional expectation

>If things do get bad, what is the expected loss?

$$
\myBox{\text{TCE}_\alpha\Pare{\tilde L}=\Exp{\tilde L\mid\tilde L\geq\VaR_\alpha\Pare{\tilde L}}  }
$$

also named

- expected shortfall
- conditional $\VaR$
- tail loss

It's the expected loss during $N$ days, conditional on the loss being greater than the $X$th percentile of the **loss distribution**

$\Rmk$

Here we use $\alpha$, to indicate that we are dealing with the *loss distribution*. Besides,
$$
\begin{align}
\text{TCE}_\alpha\Pare{\tilde L}&=\Exp{\tilde L\mid\tilde L\geq\VaR_\alpha\Pare{\tilde L}} \\
&= \int_{-\infty}^{\infty} L\times f_{\tilde L\mid\tilde L\geq\VaR_\alpha\Pare{\tilde L}}\Pare{L}\;\dd L = \int_{-\infty}^{\infty} L\; \dd F_{\tilde L\mid\tilde L\geq\VaR_\alpha\Pare{\tilde L}}\Pare{L} \\
&= \int_{-\infty}^{\infty} L\;\dd \Pare{\frac{P\Pare{\CB{\tilde L < L}\cap \CB{\tilde L\geq\VaR_\alpha\Pare{\tilde L}}}}{P\Pare{\tilde L\geq\VaR_\alpha\Pare{\tilde L}}}} \\
&= \frac{\d{\int_{-\infty}^{\infty}L f_{\tilde L}\Pare{L} \idctV_{L\geq \VaR_\alpha\Pare{\tilde L}} \;\dd L}}{P\Pare{\tilde L\geq\VaR_\alpha\Pare{\tilde L}}}= \frac{\d{\int_{-\infty}^{\infty}L\times f\Pare{L}\idctV_{L\geq \VaR_\alpha\Pare{\tilde L}}\;\dd L}}{\d{\int_{-\infty}^{\infty} f\Pare{L}\idctV_{L\geq \VaR_\alpha\Pare{\tilde L}}\;\dd L}}\\
&= \frac{\d{\int_{\VaR_\alpha\Pare{\tilde L}}^{\infty}L\times f\Pare{L}\;\dd L}}{\d{\int_{\VaR_\alpha\Pare{\tilde L}}^{\infty} f\Pare{L}\;\dd L}}\\
&= \myBox{\frac{\d{\int_{\VaR_\alpha\Pare{\tilde L}}^\infty  L\times f\Pare{L}\;\dd  L}}{1-\alpha} = \text{TCE}_\alpha\Pare{\tilde L}}
\end{align}
$$

$\eg{}$

$T=1$

two $\$10$ million loans

default probability: $\text{DP}=1.25\%$

result

- when default, loss between $0\%$ and $100\%$ are equally alike
- when not default, profit $\$0.2$ million
- one default, the other profit

$\slu$

<u>single loan</u>

<img src="D:\Notes\FinMath/Financial Risk Management_SUSTech/assets/1550790411319.png">

clearly, one year, $99\%\ \VaR$ is $\$2$ million $\implies$
$$
\begin{align}
\text{TCE}_\alpha\Pare{\tilde L}&=\Exp{\tilde L\mid\tilde L\geq\VaR_\alpha\Pare{\tilde L}}\\
&= \Exp{\tilde L\mid\tilde L \geq \$2}\\
&= \frac{\$2+\$10}{2}=\$6
\end{align}
$$

<u>consider portfolio of two loans</u>

$\text{DP}=1.25\%+1.25\%=2.5\%$

distribution

- gain, not matter
- loss, uniformly distributed from $-\$0.2$ million to $\$9.8$ million

thus here we consider from the right side

$\dfrac{1\%}{2.5\%}=0.4\implies 4$th percentile from the right is

$$
9.8-0.4\cdot\Pare{9.8-\Pare{-0.2}}=5.8 \implies
$$

similarly we have $\text{TCE}_\alpha\Pare{\tilde L}=\dfrac{\$ 5.8+\$9.8}{2}=\$7.8$

$\Rmk$ about calculation

IF loss is normally distributed, with mean $\mu$ and standard deviation $\sigma$, then we have
$$
\myBox{\begin{align}
\VaR_\alpha &= \mu+\sigma\NcN^{-1}\Pare{\alpha}\\
\text{TCE}_\alpha &= \mu+\sigma\frac{\exp\CB{-Z^2/2}}{\sqrt{2\pi}\Pare{1-\alpha}}
\end{align}}
$$
here $Z$ is the $\alpha$th percentile point of the standard normal distribution

$\Rmk$

$\VaR$ and $\text{TCE}$ share different property:

- $\VaR$: $5.8>2+2$
- $\text{TCE}$: $7.8<6+6$



$\Def$ Coherent risk measures

For these four properties: $\Ppt$

1. **Monotonicity**: return $\downarrow\implies$ risk measure $\nearrow$
2. **Translation invariance**: portfolio $\uparrow K$ cash $\implies$ risk measure $\searrow K$ 
3. **Positive homogeneity**: portfolio size factor $\lambda>0 \implies$ risk measure factor $\lambda$
4. **Subadditivity**: risk measure of portfolio $A$ and risk measure of portfolio $B$ $\geq$ risk measure of $A+B \implies$ diversification strategy

satisfying all four $\implies$ **coherent**

$\Rmk$

- $\VaR$ satisfies the first three, but not always the fourth one
- Expected shortfall $\text{TCE}$ is **coherent**

$\eg{}$

for each two

- $0.02$ of loss of $\$10$ million
- $0.98$ of loss of $\$1$ million

$\alpha=97.5$

$\slu$
$$
\begin{array}{cc}\hline
 & 97.5\%\VaR & \text{TCE}_{97.5}\\\hline
\text{single one} & \$1 & \$8.1  \\
\text{portfolio} & \$ 11 & \$ 11.144\\\hline
\end{array}
$$


$\SUM$

all risk measures we've learned till now can all be seen as a **weighted average**:
$$
\begin{array}{ccc}\hline
 & \VaR & \text{TCE}\\\hline
\text{below }\alpha\text{th} & 0 & 0 \\
\alpha\text{th} & 100\% & 0\\
\text{above }\alpha\text{th} & 0 & \text{equal weight}\\ \hline 
\end{array}
$$
weight assigned is a non-decreasing function of $\alpha\implies$ subadditivity



$\Def$ **Spectral risk measure**

a risk measure, in a weighted average form, of outcomes where worse outcomes are assigned with larger weights



### Time horizon $H$

an usual assumption is
$$
\myBox{
\begin{align}\text{N-day }\VaR &= \text{1-day }\VaR\times\sqrt{N}\\
\text{N-day TCE} &= \text{1-day TCE}\times\sqrt{N}
\end{align}}
$$
since loss are assumed to be normally distributed



### VaR: historical simulation approach

$H$: one day

$\alpha$: $99\%$

$501$ historical data

**Step**$\;\;$**1**: collect the data, shown in the picture

<img src="D:\Notes\FinMath\Financial Risk Management_SUSTech\assets\1551086094532.png" width=400>

**Step**$\;\;$**2**: calculate $500$ possible scenarios, the percentage changes of $n$ variables between day $i$ and $i+1$, $i=0,1,\dots,500$

**Step**$\;\;$**3**: calculate the possible portfolio value for each scenario, and the possible changes in portfolio value

<img src="D:\Notes\FinMath\Financial Risk Management_SUSTech\assets\1551086952321.png" width=400>

**Step**$\;\;$**4**: estimate the percentile points using the changes in value (data in last column)

for example:

- the $1$-percentile point of the distribution of *changes* in the portfolio value: the fifth-smallest number
- the $99$-percentile point of the distribution of *loss*: the negative of the fifth-smallest number
- $\myEmphy{\text{N-day }\VaR = \text{1-day }\VaR\times\sqrt{N}}$
- or even the empirical loss distribution function

$$
\myEmphy{F\Pare{x} = \frac{1}{n}\sum_i  \idctV_{\SB{0,x}}\Pare{\tilde L_p^{\Pare{i}}}}, \BBspace n=500
$$

here $L_p^{\Pare{i}}$ is the negative of the numbers in the last column



## Economic capital and risk-adjusted return on capital

$\Def$ **credit** $\VaR$

target confidence level: $\alpha$
$$
\myBox{q_\alpha=\alpha\text{-quantile of }\tilde L=\inf\CB{q>0\mid P\Pare{\tilde L \leq q}\geq \alpha}}
$$

$\Rmk$ difference of two
$$
\begin{align}
q_\alpha&=\alpha\text{-quantile of }\tilde L=\inf\CB{q>0\mid P\Pare{\tilde L \leq q}\geq \alpha}\\[0.6em]
\VaR_\alpha\Pare{\tilde L} &= \inf\CB{L\in\RR,P\Pare{\tilde L\leq L}\geq\alpha}
\end{align}
$$



$\Def$

**Economic capital** (**risk capital**) is the amount of capital a ﬁnancial institution needs to absorb losses over a certain time horizon (usually one year) with a certain conﬁdence level.

Since it's designed to cover the difference between the actual and the expected loss
$$
\text{EC}_\alpha=\text{economic capital}=q_\alpha-\text{EL}
$$
<img src="D:\Notes\FinMath\Financial Risk Management_SUSTech\assets\1551088127491.png" width=400>

$\Rmk$

Suppose $\alpha=99.98\%$

$\implies \text{EC}_\alpha$ will be sufficient to cover unexpected losses in $9998$ out of $10000$ years, assuming a planning horizon of one year

corporation rate $\uparrow\implies$ confidence level $\uparrow\implies$ $\VaR, q_\alpha\uparrow\implies\text{EC}\uparrow$



### Aggregating economic capital

IF perfect correlation between risks
$$
\text{EC}_{\text{total}} = \sum\text{EC}_i
$$
Generally it's hybrid like this
$$
\myBox{\text{EC}_{\text{total}} = \sqrt{\sum_{i=1}^n\sum_{j=1}^n \text{EC}_i\text{EC}_j \rho_{ij}  }}
$$

- exact, IF normally distributed
- approximation, IF not all normally distributed



$\eg{}$ <span id='findEC_Total'>Find</span> $\text{EC}_\text{total}$

Given estimates for economic capital
$$
\begin{array}{ccc} \hline
\text{Type of risk} & \text{Business unit 1} & \text{Business unit 2}\\\hline
\text{Market risk} & 30 & 40 \\
\text{Credit risk} & 70 & 80 \\
\text{Operational risk} & 30 & 90\\\hline
\end{array}
$$
Given their correlation
$$
\begin{array}{ccc} \hline
 & \text{MR-1}& \text{CR-1} & \text{OR-1} & \text{MR-2} & \text{CR-2} & \text{OR-2} \\\hline
\text{MR-1} & 1.0 & 0.5 & 0.2 & 0.4 & 0.0 & 0.0\\
\text{CR-1} & 0.5 & 1.0 & 0.2 & 0.0 & 0.6 & 0.0\\
\text{OR-1} & 0.2 & 0.2 & 1.0 & 0.0 & 0.0 & 0.0\\
\text{MR-2} & 0.4 & 0.0 & 0.0 & 1.0 & 0.5 & 0.2\\
\text{CR-2} & 0.0 & 0.6 & 0.0 & 0.5 & 1.0 & 0.2\\
\text{OR-2} & 0.0 & 0.0 & 0.0 & 0.2 & 0.2 & 1.0\\
\hline
\end{array}
$$
$\slu$

- Market risk: ${\text{EC}_\text{total} = \sqrt{30^2+40^2+2\times0.4\times30\times40}=58.8}$
- Credit risk: ${\text{EC}_\text{total} = \sqrt{70^2+80^2+2\times0.6\times70\times80}=134.2}$
- Operational risk: ${\text{EC}_\text{total} = \sqrt{30^2+90^2}=94.9}$
- Unit $1$: ${\text{EC}_\text{total} = \sqrt{30^2+70^2+30^2+2\times0.5\times30\times70+2\times0.2\times30\times30+2\times0.2\times70\times30}=100.0}$
- Unit $2$: ${\text{EC}_\text{total} = \sqrt{40^2+80^2+90^2+2\times0.5\times40\times80+2\times0.2\times40\times90+2\times0.2\times80\times90}=153.7}$

$$
\text{EC}_\text{total}=\sqrt{\begin{align}
&30^2+40^2+70^2+80^2+30^2+90^2\\
+\; &2\times0.5\times30\times70 + 2\times0.2\times30\times30\\
+\; &2\times0.4\times30\times40 + 2\times0.2\times70\times30\\
+\; &2\times0.6\times70\times80 + 2\times0.5\times40\times80\\
+\; &2\times0.2\times40\times90 + 2\times0.2\times80\times90
\end{align}} = 203.224
$$

$\Rmk$

Clearly,
$$
58.8+134.2+94.9=287.9>100.0+153.7=253.7>203.224
$$



### Risk-adjusted return on capital

$\Def$ RAROC and RAPM

Risk-adjusted return on capital (RAROC):
$$
\myBox{\text{RAROC} = \frac{\text{Revenues}-\text{Costs}-\text{EL}}{\text{EC}}}
$$
this is one of the Risk-adjusted performance measurement (RAPM).

$\eg{}$

a loan,

its losses: $1\%$ of outstanding loans per year on average

$99.9\%$ worst-case loss: $5\%$ of outstanding loans

spread between the cost of funds and the interest charged: $2.5\%$

administrative cost: $0.7\%$

$\slu$

Suppose there's $\$100$ of loan
$$
\text{EC} = q_{99.9\%}-\text{EL}=5\%\cdot M-1\%\cdot M = \$4\\
\text{RAROC} = \frac{2.5\%\cdot M-0.7\%\cdot M-1\%\cdot M}{\$4}=\frac{0.8}{4}=20\%\\
$$
$\Rmk$

An alternative approach:
$$
\text{RAROC}  = \frac{\text{Revenues}-\text{Costs}-\text{EL}}{\text{EC}}+r_f
$$
IF risk free interest rate: $2\%$
$$
\text{RAROC}^* =20\%+2\%=22\%
$$


### Impact of autocorrelation on Value-at-Risk

Recall: $\myEmphy{\text{N-day VaR}=\text{1-day VaR}\times \sqrt N}$

This will fail when autocorrelation exists.

$\Zrm$ Autocorrelation model for changes of portfolio value

$i$: date

$V_i$: value of portfolio

$\sigma^2$: $\Var{\Delta V_i}$, $\forall\; i$

Suppose: **first order autocorrelation**
$$
\myBox{\Delta V_i = \rho \Delta V_{i-1}+a_i}
$$
for all $i$, and here $a_i$ satisfy:

- $\Exp{a_i}=0$, zero mean
- $\Var{a_i}=\tilde\sigma^2$, constant variance
- $\Cov{a_i,a_{i-k}}=0$, $\forall \; k\neq 0$

$\implies$
$$
\myBox{\Var{\sum_{i=1}^N \Delta V_i} = \sigma^2\SB{N+2\Pare{N-1}\rho+2\Pare{N-2}\rho^2+\cdots+2\rho^{N-1}}}
$$

$$
\implies\myBox{\text{N-day VaR}=\text{1-day VaR}\times \sqrt{N+2\Pare{N-1}\rho+2\Pare{N-2}\rho^2+\cdots+2\rho^{N-1}}   }
$$

$\pf$

$\QQQ \Cov{a_i,\Delta V_k}=0$, $\forall \; k<i$ 
$$
\begin{align}
\Cov{\Delta V_i,\Delta V_{i-k}} &= \rho\,\Cov{\Delta V_{i-1},\Delta V_{i-k}} + \Cov{a_i,\Delta V_{i-k}}\\
&= \rho^2 \,\Cov{\Delta V_{i-2},\Delta V_{i-k}}\\
&= \rho^k\,\Cov{\Delta V_{i-k},\Delta V_{i-k}}=\rho^k\sigma^2
\end{align}
$$

$$
\begin{align}
\Var{\sum_{i=1}^N \Delta V_i} &= \sum_{i=1}^N\sum_{j=1}^N \Cov{\Delta V_i,\Delta V_j}\\
&= \begin{array}{cccccccccc}
&\sigma^2&+&\rho\sigma^2&+&\rho^2\sigma^2&+&\cdots&+&\rho^{N-2}\sigma^2&+&\rho^{N-1}\sigma^2 \\
+&\rho\sigma^2&+&\sigma^2&+&\rho\sigma^2&+&\cdots&+&\rho^{N-3}\sigma^2&+&\rho^{N-2}\sigma^2\\
+&\rho^2\sigma^2&+&\rho\sigma^2&+&\sigma^2&+&\cdots&+&\rho^{N-4}\sigma^2&+&\rho^{N-3}\sigma^2\\
&\vdots&&\vdots&&\vdots&&&&\vdots&&\vdots&&\\
+&\rho^{N-1}\sigma^2&+&\rho^{N-2}\sigma^2&+&\rho^{N-3}\sigma^2&+&\cdots&+&\rho\sigma^2&+&\sigma^2
\end{array}\\[0.8em]
&= \sigma^2\SB{N+2\Pare{N-1}\rho+2\Pare{N-2}\rho^2+\cdots+2\rho^{N-1}}
\end{align}
$$

$\QED$



### Marginal, incremental and component Value-at-Risk

Recall: [Risk contribution](#Risk-contribution): $\d{\myEmphy{\text{RC}_i = \text{UL}_i \frac{\partial \text{UL}_p}{\partial\text{UL}_i}} \implies\myEmphy{\text{UL}_p = \sum_i \text{RC}_i}}$

$\Def$ Marginal $\VaR$, Incremental $\VaR$, Component $\VaR$

portfolio with components

$i\texttt{-th}$ component

$x_i$: investment in $i\texttt{-th}$ component

<u>marginal</u>

the sensitivity of $\VaR $ to the amount invested in the $i\texttt{-th}$ component.

$\implies$
$$
\myBox{\text{marginal VaR} = \frac{\partial\VaR}{\partial x_i}}
$$

<u>incremental</u>

> What is the difference between $\VaR$ with and without the trade?

could be

- the incremental effect on $\VaR$ of a new trade
- the incremental effect on $\VaR$ of closing out an existing trade

$\implies$
$$
\myBox{\text{incremental VaR} =\VaR\Pare{x_i=\epsilon}-\VaR\Pare{x_i=0} \approx \frac{\partial\VaR}{\partial x_i}x_i} = C_i
$$

<u>component</u>

the part of $\VaR$ that can be attributed to this component

$\implies$

$$
\myBox{\text{component VaR} = \frac{\partial\VaR}{\partial x_i}x_i=C_i}
$$


$\Def$ linear homogeneity

$V$: risk measure

$x_i$: investment in $i\texttt{-th}$ component

IF $x_i$ is changed to $\lambda x_i$, $\forall\; i$

then $V$ changes to $\lambda V$

$\implies$ $V$ satisfies the linear homogeneity condition

$\Def$ homogenous function of degree one

$x_1,\dots,x_n$: variables

$f\Pare{x_1,\dots,x_n}$: continuous and differentiable function

IF $\forall \; c$, constant,

then $f\Pare{c\cdot x_1,\dots,c\cdot x_n} =c\cdot f\Pare{x_1,\dots,x_n}$

$\implies$ $f$ is homogenous function of degree one

$\Zrm$ Euler's theorem

$x_1,\dots,x_n$: variables

$f\Pare{x_1,\dots,x_n} = f\Pare{\mathbf x}$: differentiable and homogenous of degree one function

$\implies$
$$
\myEmphy{f\Pare{\mathbf x}=x_1\cdot\frac{\partial f\Pare{\mathbf x}}{\partial x_1}+x_2\cdot\frac{\partial f\Pare{\mathbf x}}{\partial x_2}+\cdots+x_n\cdot\frac{\partial f\Pare{\mathbf x}}{\partial x_2}= \Tran{\mathbf x}\frac{\partial f\Pare{\mathbf x}}{\partial \mathbf x} }
$$
$\pf$

$\QED$

$\Corlr$

Euler's theorem$\implies$
$$
\myBox{\VaR = \sum_i\frac{\partial\VaR}{\partial x_i}x_i=\sum_i C_i }
$$
$\pf$

2333

$\QED$

$\Rmk$

$C_i$ can also be regarded as the *expected loss* on the $i\texttt{-th}$ position, conditional on the loss of the portfolio equaling the $\VaR$ level
$$
\QQQ\myBox{C_i = \Exp{\tilde L_i\mid \tilde L = \VaR}}
$$


$\Rmk$

Here we can similarly obtain
$$
\myBox{\text{EC} = \sum_i \frac{\partial\text{EC}}{\partial x_i}x_i}
$$

### Allocation of the diversification benefit

$i\texttt{-th}$ business unit

$x_i$: investment

$\implies$ allocate $\dfrac{\partial\text{EC}}{\partial x_i}x_i$ to the $i\texttt{-th}$ business unit

$\implies$ approximation
$$
\myBox{\dfrac{\partial\text{EC}}{\partial x_i}x_i\approx \frac{\Delta\text{EC}}{\Delta y_i }}\BBspace y_i=\frac{\Delta x_i}{x_i}
$$
$\eg{}$

see [previous](#findEC_Total)

$\text{EC}_{\text{total}}=203.2$, $\text{EC}_1=100$, $\text{EC}_2=153.7$

now allocate

$\slu$

<u>naive</u>
$$
\begin{array}{ccc}\hline
\text{Unit}&\text{Business unit 1} & \text{Business unit 2}\\\hline
\text{Portion} & \dfrac{100}{100+153.7} & \dfrac{153.7}{100+153.7} \\
\text{Investment} & 80.1 & 123.1\\ \hline
\end{array}
$$
<u>incremental effect approach</u>
$$
\begin{array}{ccc}\hline
\text{Unit}&\text{Business unit 1} & \text{Business unit 2}\\\hline
\text{Incremental effect}& 203.2-153.7 & 203.2 − 100\\
\text{Portion} & \dfrac{49.5}{49.5+103.2} & \dfrac{103.2}{49.5+103.2} \\
\text{Investment} & 65.9 & 137.3\\ \hline
\end{array}
$$
$\myEmphy{\dfrac{\Delta\text{EC}}{\Delta y_i }}$

let

$\Delta y_i=1\%$
$$
\begin{array}{ccc} \hline
\text{Type of risk} & \text{Business unit 1}\Pare{+1\%} & \text{Business unit 2}\Pare{+1\%}\\\hline
\text{Market risk} & 30.3 & 40.4 \\
\text{Credit risk} & 70.7 & 80.8 \\
\text{Operational risk} & 30.3 & 90.9\\\hline
\end{array}
$$

$$
\text{EC}_\text{total,unit 1+}=\sqrt{\begin{align}
&30.3^2+40^2+70.7^2+80^2+30.3^2+90^2\\
+\; &2\times0.5\times30.3\times70.7 + 2\times0.2\times30.3\times30.3\\
+\; &2\times0.4\times30.3\times40 + 2\times0.2\times70.7\times30.3\\
+\; &2\times0.6\times70.7\times80 + 2\times0.5\times40\times80\\
+\; &2\times0.2\times40\times90 + 2\times0.2\times80\times90
\end{align}} = 203.906351
$$

$$
\text{EC}_\text{total,unit 2+}=\sqrt{\begin{align}
&30^2+40.4^2+70^2+80.8^2+30^2+90.9^2\\
+\; &2\times0.5\times30\times70 + 2\times0.2\times30\times30\\
+\; &2\times0.4\times30\times40.4 + 2\times0.2\times70\times30\\
+\; &2\times0.6\times70\times80.8 + 2\times0.5\times40.4\times80.8\\
+\; &2\times0.2\times40.4\times90.9 + 2\times0.2\times80.8\times90.9
\end{align}} = 204.576543
$$

$$
\begin{array}{ccc}\hline
\text{Unit}&\text{Business unit 1} & \text{Business unit 2}\\\hline
\text{Incremental}& 1\% & 1\%\\
{\Delta\text{EC}} & 0.682 & 1.353 \\
\text{Investment} & 68.2 & 135.3\\ \hline
\end{array}
$$

$\Rmk$

Other allocation schemes exist.

The best are those that reflect the **incremental impact** of the business unit on the **total economic capital**.

The amount of capital allocated to a business unit is generally *less than* the capital estimated for the business unit as a stand-alone entity because of diversification benefits.