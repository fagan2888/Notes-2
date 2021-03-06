# Conditional Probability and Independence

Yuanxing Cheng, May 12, 2020
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
\DeclareMathOperator*{\trace}{Trace}
\newcommand{\space}{\;\;}
\newcommand{\bspace}{\;\;\;}
\newcommand{\Bspace}{\;\;\;\;}
\newcommand{\bbspace}{\;\;\;\;\;}
\newcommand{\BBspace}{\;\;\;\;\;\;}
\newcommand{\QbQQ}{\boxed{?\:}}
\newcommand{\void}{\left.\right.}
% latex Emphy
% \definecolor{EmphyQ}{HTML}{880015}
% \definecolor{EmphyW}{HTML}{660066}
%\newcommand{\myEmphy}[2][EmphyQ]{ {\color{#1}{#2}} }
%\newcommand{\myBox}[2][9px, border:2px solid EmphyQ]{ {\bbox[#1]{#2}} }
% markdown Emphy
\newcommand{\myEmphy}[2][#880015]{ {\color{#1}{#2}} }
\newcommand{\myBox}[2][9px, border:2px solid #880015]{ {\bbox[#1]{#2}} }
\newcommand{\d}[1]{ {\displaystyle{#1}} }
\newcommand{\CB}[1]{\left\{ #1 \right\}}
\newcommand{\SB}[1]{\left[ #1 \right]}
\newcommand{\Pare}[1]{\left( #1 \right)}
\newcommand{\AB}[1]{\left \langle #1 \right \rangle}
\newcommand{\abs}[1]{\left| #1 \right|}
\newcommand{\norm}[1]{\left\| #1 \right\|}
\newcommand{\given}[1]{\left. #1 \right|}
\newcommand{\using}[2][=]{\overset{\mathrm{#2}}{#1}}
\newcommand{\usingUD}[3][=]{\underset{\text{#2}}{\overset{\text{#3}}{#1}}}
\newcommand{\asim}{\overset{\text{a}}{\sim}}
\newcommand{\tinyText}[1]{ {\tiny{\text{#1}}} }
\newcommand{\scriptsizeText}[1]{ {\scriptsize{\text{#1}}} }
\newcommand{\footnotesizeText}[1]{ {\footnotesize{\text{#1}}} }
\newcommand{\smallText}[1]{ {\small{\text{#1}}} }
\newcommand{\largeText}[1]{ {\large{\text{#1}}} }
\newcommand{\LargeText}[1]{ {\Large{\text{#1}}} }
\newcommand{\LARGEText}[1]{ {\LARGE{\text{#1}}} }
\newcommand{\hugeText}[1]{ {\huge{\text{#1}}} }
\newcommand{\HugeText}[1]{ {\Huge{\text{#1}}} }
\newcommand{\AbA}{\mathbb{A}}
\newcommand{\RbR}{\mathbb{R}}
\newcommand{\EbE}{\mathbb{E}}
\newcommand{\FbF}{\mathbb{F}}
\newcommand{\GbG}{\mathbb{G}}
\newcommand{\HbH}{\mathbb{H}}
\newcommand{\IbI}{\mathbb{I}}
\newcommand{\NbN}{\mathbb{N}}
\newcommand{\ZbZ}{\mathbb{Z}}
\newcommand{\QbQ}{\mathbb{Q}}
\newcommand{\PbP}{\mathbb{P}}
\newcommand{\AcA}{\mathcal{A}}
\newcommand{\BcB}{\mathcal{B}}
\newcommand{\CcC}{\mathcal{C}}
\newcommand{\DcD}{\mathcal{D}}
\newcommand{\EcE}{\mathcal{E}}
\newcommand{\FcF}{\mathcal{F}}
\newcommand{\GcG}{\mathcal{G}}
\newcommand{\HcH}{\mathcal{H}}
\newcommand{\IcI}{\mathcal{I}}
\newcommand{\NcN}{\mathcal{N}}
\newcommand{\RcR}{\mathcal{R}}
\newcommand{\YcY}{\mathcal{Y}}
\newcommand{\ZcZ}{\mathcal{Z}}
\newcommand{\AsA}{\mathscr{A}}
\newcommand{\FsF}{\mathscr{F}}
\newcommand{\IsI}{\mathscr{I}}
\newcommand{\idct}{\mathbf{1}}
\newcommand{\dd}{\mathrm{d}}
\newcommand{\Tran}[1]{{#1}^{\mathrm{T}}}
\newcommand{\reff}[1]{ \tag{#1}\label{#1} }
\newcommand{\reft}[1]{ \Pare{\ref{#1}} }
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
\newcommand{\hess}{\mathrm{Hess}}
\newcommand{\ow}{\text{otherwise}}
\newcommand{\wp}{\text{with probability }}
\newcommand{\FSD}{\text{FSD}}
\newcommand{\SSD}{\text{SSD}}
\newcommand{\QED}{\myEmphy{\blacksquare}}
\newcommand{\SUM}{\myEmphy{\text{Summary}}}
\newcommand{\pf}{\myEmphy{\largeText{Proof}}}
\newcommand{\slu}{\myEmphy{\largeText{Solution}}}
\newcommand{\Corlr}[1]{\myEmphy{\largeText{Corrollary #1}}}
\newcommand{\Corlr}{\myEmphy{\largeText{Corrollary}}}
\newcommand{\rmk}[1]{\myEmphy{\largeText{Remark #1}}}
\newcommand{\Rmk}{\myEmphy{\largeText{Remark}}}
\newcommand{\pops}[1]{\myEmphy{\largeText{Proposition #1}}}
\newcommand{\Pops}{\myEmphy{\largeText{Proposition}}}
\newcommand{\zrm}[1]{\myEmphy{\largeText{Theorem #1}}}
\newcommand{\Zrm}{\myEmphy{\largeText{Theorem}}}
\newcommand{\PPt}[1]{\myEmphy{\largeText{Property #1}}}
\newcommand{\PPt}{\myEmphy{\largeText{Property}}}
\newcommand{\def}[1]{\myEmphy{\largeText{Definition #1}}}
\newcommand{\Def}{\myEmphy{\largeText{Definition}}}
\newcommand{\lm}[1]{\myEmphy{\largeText{Lemma #1}}}
\newcommand{\Lm}{\myEmphy{\largeText{Lemma}}}
\newcommand{\eg}[1]{\myEmphy{\largeText{Example #1}}}
\newcommand{\ex}[1]{\myEmphy{\largeText{Exercise #1}}}
$$
$\def{3.1}$ 

- Two events $A$ and $B$ (subsets of $\Omega$) are ***independent*** if $P\Pare{A\cap B}=P\Pare A \cdot P\Pare B$
- A collection of events $\Pare{A_i}_{i\in I}$ is an ***independent*** collection  if for every finite subset $J$ of $I$, $P\Pare{\bigcap_{i\in J} A_i}=\prod_{i\in J}P\Pare{A_i}$. Here it's also called ***mutually independent***.

$\Rmk$ Independent$\implies$pairwise independent

$\zrm{3.1}$ If $A$ and $B$ are independent, then so are $A$ and $B^c$, $A^c$ and $B$, $A^c$ and $B^c$

$\def{3.2}$ Let $A$, $B$ be events, $P\Pare{B}>0$.

The ***conditional probability*** of $A$ given $B$ is $P\Pare{A\mid B}=\dfrac{P\Pare{A\cap B}}{P\Pare B}$.

$\zrm{3.2}$ Suppose $P\Pare B>0$

- $A$ and $B$ are independent$\iff P\Pare{A\mid B}=P\Pare A$
- the mapping: $A\mapsto P\Pare{A\mid B}$ from $\AcA\to\SB{0,1}$ is a new probability measure on $\AcA$, called the ***conditional probability measure given*** $B$

$\zrm{3.3}$ If $A_1,\dots,A_n\in\AcA$ and $P\Pare{A_1\cap\cdots\cap A_{n-1}}>0$ then
$$
P\Pare{A_1\cap\cdots\cap A_n}=P\Pare{A_1}P\Pare{A_2\mid A_1}P\Pare{A_3\mid A_1\cap A_2}\cdots P\Pare{A_n\mid A_1\cap \cdots\cap A_{n-1}}
$$


$\Def$ A collection of events $\Pare{E_n}$ is called a ***partition*** of $\Omega$ if:

- $E_n\in\AcA$, for each $n$
- $E_n$ are pairwise disjoint
- $P\Pare{E_n}>0$, for each $n$
- $\cup_n E_n=\Omega$

$\zrm{3.4 (Partition Equation)}$ Let $\Pare{E_n}$ be a finite or countable partition of $\Omega$. Then if $A\in\AcA$,
$$
P\Pare{A}=\sum_n P\Pare{A\mid E_n}\cdot P\Pare{E_n}
$$
$\pf$ $A=A\cap \Omega=A\cap\Pare{\cup_n E_n}=\cup_n\Pare{A\cap E_n}$.

$\zrm{3.5 (Bayes' Theorem)}$ Let $\Pare{E_n}$ be a finite or countable partition of $\Omega$. Supposing $P\Pare A>0$, then


$$
P\Pare{E_n\mid A}=\frac{P\Pare{A\mid E_n}\cdot P\Pare{E_n}}{\sum_m P\Pare{A\mid E_m}\cdot P\Pare{E_m}}
$$


## Exercises

In all exercises the probability space is fixed, and $A$, $B$, $A_n$, etc. are events.

$\ex{3.1}$ Show that if $A\cap B=\O$ then $A$ and $B$ cannot be independent unless $P\Pare A=0$ or $P\Pare{B}=0$.

$\ex{3.2}$ Let $P\Pare C>0$. Show $P\Pare{A\cup B\mid C}=P\Pare{A\mid C}+P\Pare{B\mid C}-P\Pare{A\cap B\mid C}$.

$\ex{3.3}$ Let $P\Pare C>0$ and $A_1,\dots,A_n$ are pairwise disjoint. Show that $P\Pare{\cup_{i=1}^n A_i\mid C}=\sum_{i=1}^n P\Pare{A_i\mid C}$.

$\ex{3.4}$ Let $P\Pare C>0$. Show $P\Pare{A\cap C}=P\Pare{A\mid C}\cdot P\Pare C$.

$\ex{3.5}$ Let $0<P\Pare{C}<1$ and $A$ be any event. Show $P\Pare A=P\Pare{A\mid C}\cdot P\Pare C+P\Pare{A\mid C^c}\cdot P\Pare{C^c}$.

$\ex{3.6}$ nah

$\ex{3.7}$ Let $\Pare{A_n}_{n\geq 1}\in\AcA$ and $\Pare{B_n}_{n\geq 1}\in\AcA$ and $A_n\to A$, $B_n\to B$, with $P\Pare B>0$ and $P\Pare{B_n}>0$, for all $n$. Show:

1. $\lim_{n\to\infty}P\Pare{A_n\mid B}=P\Pare{A\mid B}$
2. $\lim_{n\to\infty}P\Pare{A\mid B_n}=P\Pare{A\mid B}$
3. $\lim_{n\to\infty}P\Pare{A_n\mid B_n}=P\Pare{A\mid B}$

$\pf$ notice that $\idct_{A\cap B}\Pare{\omega}=\idct_A\Pare\omega\cdot\idct_{B}\Pare\omega$

and more on 1), since $P\Pare{\cdot\mid B}$ is a probability measure thus by Theorem 2.4, it's obvious.

$\ex{3.8}$ nah

$\ex{3.9}$ Suppose $A,B,C$ are independent events and $P\Pare{A\cap B}\neq 0$. Show $P\Pare{C\mid A\cap B}=P\Pare C$.

$\ex{3.10~3.16}$ nah

$\ex{3.17}$ Let $A_1,A_2,\dots,A_n$ be independent events. Show that the probability that none of the $A_1,\dots,A_n$ occur is less than or equal to $\exp\CB{-\sum_{i=1}^n P\Pare{A_i}}$

$\pf$ use $1+x\leq e^{x}$

$\ex{3.18}$ Let $A,B$ be events with $P\Pare{A}>0$. Show $P\Pare{A\cap B\mid A\cup B}\leq P\Pare{A\cap B\mid A}$.