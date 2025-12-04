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

## 1) Discrete Random Variables
Classified based on countability as, 
1) Countably Infinite.
1) Countably Finite.

### Probability Density Function (PDF) / Probability Mass Function (PMF)
|x|0|1|2|...|n|
|-|-|-|-|-|-|
|\\(P(x=x)\\)|\\(p_0\\)|\\(p_1\\)|\\(p_2\\)|\\(...\\)|\\(p_n\\)|
> [!NOTE]
>\\[ \sum{P(x)} = 1\\]

### Mean / Expectation 
\\[
E(x) = \sum{xP(x)}
\\]
### Variance
Variance of `x`: \\(
var(x) = E(x^2) - [E(x)]^2
\\)<br>
Variance of `ax+n`: \\(
var(ax + b) = a^2var(x) + 0 = a^2var(x)
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

### Cumulative Distribution Function (CDF)

