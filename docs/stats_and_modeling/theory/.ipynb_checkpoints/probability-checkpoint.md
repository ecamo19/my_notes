# Probability

[ref](https://www.codecademy.com/paths/fundamental-math-for-data-science/tracks/math-ds-probability/modules/math-ds-rules-of-probability/articles/probability-set-theory-and-the-law-of-large-numbers)

## Set theory
Set is a collection of things. For example, we can use a set to represent items in a backpack. An example of a set could be: $${Book,Paper,Folder,Hat,Pen,Snack}$$

Sets also follow two key rules:
+ Each element in a set is distinct.
+ The elements in a set are in no particular order.

Sets can also contain subsets. Set A is a subset of set B if all the elements in A exist within B. For example:

$$A = {1,2,3}$$
$$B = {1,2,3,4,5}$$

## Experiments and Sample Spaces

In probability, an __experiment__ is something that produces observation(s) with some level of uncertainty. 

A __sample point__ is a single possible outcome of an experiment. 

Finally, a __sample space__ is the set of all possible sample points for an experiment.


For example, suppose that we run __an experiment__ where we flip a coin twice and record whether each flip results in heads or tails. There are four sample points in this experiment: two heads (HH), tails and then heads (TH), heads and then tails (HT), or two tails (TT). We can write the full __sample space__ for this experiment as follows:

$$S = \{HH, TT, HT, TH\}$$

Suppose we are interested in the probability of one specific outcome: _HH_. A specific outcome (or set of outcomes) is known as an event and is a subset of the sample space. Three events we might look at in this sample space are:

$$Getting\ Two\ Heads$$
$$A={HH}$$
$$Getting\ Two\ Tails$$
$$B={TT}$$
$$Getting\ Both\ a\ Heads\ and\ Tails$$
$$C={HT,TH}$$

## The frequentist definition of probability 

If we run an experiment an infinite amount of times, the probability of each event is the proportion of times it occurs. Unfortunately, we don’t have the ability to flip two coins an infinite amount of times — but we can estimate probabilities by choosing some other large number, such as 1000. For example:

$${HH}: 252$$
$${TT}: 247$$
$${HT}: 256$$
$${TH}: 245$$



To calculate the estimated probability of any one outcome, we use the following formula:

$$P(event) = \frac{Number\ of\ times\ the\ event\ occurred}{Total\ number\ of\ trials}$$

In this scenario, a trial is a __single run__ of our experiment (two coin flips). So, the probability of two heads on two coin flips is approximately:

$$P(HH) = \frac{255}{1000}$$

## Law of Large Numbers
We can’t repeat our random experiment an infinite amount of times. However, we can still flip both coins a large number of times. As we flip both coins more and more, the observed proportion of times each event occurs will converge to its true probability. This is called the law of large numbers.


Let’s observe the law of large numbers in real-time


```{python}

print("hello")

```









































