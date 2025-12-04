# Module 1 - Discrete Probability Distribution
## Definitions

|Term| Definition|
|------|-------|
|Random Experiment|An experiment in which, all outcomes are known in advance but the output cannot be predicted.|
|Sample Space (S)| The set of all possible outcomes.|
|Random Variable (RV)| A rule that associates a number with an outcome. \\(f: S \to \mathbb{R}\\)|
|Exhaustive Event| A collection of events whose union is the sample space.|
|Exclusive Event| A collection of events whose pairwise intersection is \\(\phi\\)|

> [!NOTE]
>\\[
>0 \le P(A) \le 1
>\\]
>\\[
>P(A) = 1 - P(\overline{A}) 
>\\]
>\\[
P(A) + P(\overline{A}) = 1
>\\]

## Random Variables (RV)
Random variables are of 2 types.
1) Discrete Random Variable (DRV)
2) Continuous Random Variable (CRV)

## Discrete Random Variables
Classified based on countability as, 
1) Countably Infinite.
1) Countably Finite.

## Probability Distribution Function / Probability Mass Function (PMF)
|x|0|1|2|...|n|
|-|-|-|-|-|-|
|\\(P(x=x)\\)|\\(p_0\\)|\\(p_1\\)|\\(p_2\\)|\\(...\\)|\\(p_n\\)|
> [!NOTE]
>\\[ \sum{P(x)} = 1\\]

## Mean / Expectation 
\\[
E(x) = \sum{xP(x)}
\\]
## Variance
Variance of `x`: \\(
var(x) = E(x^2) - [E(x)]^2
\\)<br>
Variance of `ax+n`: \\(
var(ax + b) = a^2var(x) + 0 = a^2var( x)
\\)

### Questions
#### Q. Find the number of heads when 3 coins are tossed.
<details>
  <summary>Answer</summary>
  \[S = \{TTT, TTH, THT, THH, HTT, HTH, HHT, HHH\}\]

  | X | 0 | 1 | 2 | 3 |
  |---|---|---|---|---|
  | \\(P(x = x)\\) | \\(\frac{1}{8}\\) | \\(\frac{3}{8}\\) | \\(\frac{3}{8}\\) | \\(\frac{1}{8}\\) |
  
</details>

#### Q. Each rod produced by a factory is inspected for surface defects.

  | X | -2 | -1 | 0 | 1 | 2 | 3 |
  |---|----|----|---|---|---|---|
  | \\(P(x = x)\\) | \\(0.1\\) | \\(15k^2\\) | \\(0.2\\) | \\(2k\\) |\\(0.3\\)|\\(3k\\)|
#### Find the value of k
  

<details>
  <summary>Answer</summary><br>
  \(0.1+0.2+0.3+2k+3k+15k^2 = 15k^2+5k+0.6 = 1 \) <br>
  \(15k^2+5k=0.4\) <br>
  \(k = \frac{1}{15}\)

  > [!NOTE]
  >The roots are: \\(\frac{1}{15}\\) and \\(\frac{-2}{5}\\), but probability cannot be negative, so we take \\(\frac{1}{15}\\).

  | X | -2 | -1 | 0 | 1 | 2 | 3 |
  |---|----|----|---|---|---|---|
  | \\(P(x = x)\\) | \\(0.1\\) | \\(\frac{1}{15}\\) | \\(0.2\\) | \\(\frac{2}{15}\\) |\\(0.3\\)|\\(\frac{1}{5}\\)|

 \\(Variance = \sigma^2 =  2.456\\)<br>
 \\(SD = \sigma =  1.567\\)
</details>

## Cumulative Distribution Function (CDF)
Represented as \\(F(x)\\) or \\(P(x \le x)\\)
\\[\sum_{x \le x}{f(x)}\\]

### Questions
#### Q. Two coins are tossed, x is the number of heads. Find CDF.
<details>
  <summary>Answer</summary>

  | X | 0 | 1 | 2 | 
  |---|---|---|---|
  | \\(P(x = x)\\) | \\(\frac{1}{4}\\) | \\(\frac{1}{2}\\) | \\(\frac{1}{4}\\) |
  | \\(P(x \le x)\\)| \\(\frac{1}{4}\\) | \\(\frac{3}{4}\\) | \\(1\\) |
  
</details>

#### Q. A store carries flash drives with 1Gb, 2Gb, 4Gb, 8Gb and 16Gb of memory. The following table gives the distribution of purchased memory.
 | Y | 1 | 2 | 4 | 8 | 16 |
 |---|---|---|---|---|----|
 |\\(P(x=x)\\)| \\(0.05\\) |\\(0.1\\)|\\(0.35\\)|\\(0.4\\)|\\(0.1\\)|

<details>
  <summary>Answer</summary>

 | Y | 1 | 2 | 4 | 8 | 16 |
 |---|---|---|---|---|----|
 |\\(P(x=x)\\)| \\(0.05\\) |\\(0.1\\)|\\(0.35\\)|\\(0.4\\)|\\(0.1\\)|
 |\\(P(x \le x)\\)| \\(0.05\\) |\\(0.15\\)|\\(0.5\\)|\\(0.9\\)|\\(1\\)|

<br>

As a function, 
  \\(
F(x) =
\begin{cases}
0 & y < 1 \\\\
0.05 & 1 \le y < 2 \\\\
0.15 & 2 \le y < 4 \\\\
0.5 & 4 \le y < 8 \\\\
0.9 & 8 \le y < 16 \\\\
1 & y \ge 16
\end{cases}
\\)

</details>

#### Q. Find k and therefore the CDF
 | X | -2 | -1 | 0 | 1 | 2 | 3 |
 |---|----|----|---|---|---|---|
 |\\(P(x=x)\\)| \\(0.1\\) |\\(k\\)|\\(0.2\\)|\\(2k\\)|\\(0.3\\)| \\(3k\\)|

<details>
  <summary>Answer</summary>

\\(0.1+0.2+0.3+k+2k+3k = 1\\)<br>
\\(6k = \frac{4}{10}\\)<br>
\\(k = \frac{1}{15}\\)
 | X | -2 | -1 | 0 | 1 | 2 | 3 |
 |---|----|----|---|---|---|---|
 |\\(P(x=x)\\)| \\(0.1\\) |\\(\frac{1}{15}\\)|\\(0.2\\)|\\(\frac{2}{15}\\)|\\(0.3\\)| \\(\frac{1}{5}\\)|
 |\\(P(x \le x)\\)| \\(\frac{1}{10}\\) |\\(\frac{1}{5}\\)|\\(\frac{11}{30}\\)|\\(\frac{1}{2}\\)|\\(\frac{4}{5}\\)| \\(1\\)|
</details>

#### Q. Computer system records the response times of a server as `X`. CDF is given.
\\(
F(x) =
\begin{cases}
0 & x < 0 \\\\
\frac{1}{4} & 0 \le x < 1 \\\\
\frac{1}{2} & 1 \le x < 3 \\\\
\frac{3}{4} & 3 \le x < 5 \\\\
1 & x \ge 5
\end{cases}
\\)



