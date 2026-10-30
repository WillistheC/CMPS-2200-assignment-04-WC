# CMPS 2200 Assignment 4
## Answers

**Name:**_________________________

Place all written answers from `assignment-04.md` here for easier grading.


**1 Quicksort probabilities**

- **1a. (5 pts)** What is the probability that Quicksort does $\Omega({n^2})$
  comparisons? 

  $\mathbf{P}[X \geq n^{2}] \leq \frac{nlogn}{n^2} = \frac{logn}{n}$


- **1b. (5 pts)** What is the probability that Quicksort does $10^c n \lg n$
comparisons, for a given $c>0$? What does this say about the
deviation of the actual work from the expected work for Quicksort?

  $\mathbf{P}[X \geq 10^{c}nlogn] \leq \frac{nlogn}{10^{c}nlogn} = \frac{1}{10^{c}}$

  The probability of the deviation gets lower the greater the size of the deviation is, and the greater $n$ is

**2 From "Maybe" to "Definitely"**

- **2a. (10 pts)** Give an algorithm to improve the guaranteed success probability and state its work.

  $\mathcal{A}'(\mathcal{I}, \delta)$ should be implented by running $\mathcal{A}(\mathcal{I}), checking its output using $\mathcal{C}, returning the result if its correct, and repeating it until there is a correct output (call this at least $k$ times)

  So, $\mathcal{P}$(success with $k$ attempts) $= 1 - (1 - \epsilon)^{k}$


- **2b. (6 pts)** Show how to convert $\mathcal{A}$ into an
  algorithm that always produces the correct result, but has an
  expected runtime that depends on $w(n)$ and a success probability
  $\epsilon$.

**3 Determinism versus Randomization in Quicksort**


- **3b. (8 pts)** Compare running times using `compare-qsort` between variants of
Quicksort and the provided implementation of selection sort (`ssort`).




- **3c. (8 pts)** Compare the fastest of your sorting implementations to the Python sorting function `sorted`, conducting the tests in 3b above. 
