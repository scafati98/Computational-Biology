# Computational-Biology

Formally, an HMM is defined by: an alphabet of emitted symbols; a set of k (hidden) states;
a matrix of state transition probabilities and a matrix of emission probabilities. In this case
we consider an HMM model with three states, to identify DNA coding regions: state 1 corresponds to
the Start Site Signal, state 2 coressponds to Exon region and state 3 corresponds to an Intron region.
We consider Initial probabilities for all the three states equal and transitions from all the states to an
end state are also equal.

Define the transition probabilities in the transition probabilities matrix.
Define the sequence on the 'sequence' string. 
We use logarithm to compute probabilties to make it robust for longer sequences.

Input:

A DNA sequence X.

Output:

A path that maximizes the probabilty over all possible paths, for the given HMM model.

We use Viterbi Algorithm to solve the last, Forward algorithm to compute the probability of the sequence
and Backward algorithm to compute the posterior probabilities for given positions.
