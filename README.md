# turing completeness
exploring the idea of Turing Completeness

Entscheidungsproblem: The problem to decide for every statement in first-order logic whether or not it is derivable in that logic.

Note that in its original form (Hilbert & Ackermann 1928), the problem was stated in terms of validity rather than derivability. Given Gödel’s completeness theorem (Gödel 1929) proving that there is an effective procedure (or not) for derivability is also a solution to the problem in its validity form. In order to tackle this problem, one needs a formalized notion of “effective procedure” and Turing’s machines were intended to do exactly that.

## The Entscheidungs problem
### may be stated in the following three equivalent ways:

- (1) Find an algorithm to determine whether a given sentence of first order logic
is valid, that is, true regardless of what speciic objects and relationships are
being reasoned about.

- (2) Find an algorithm to determine whether a given sentence of first order logic
is satisiable, that is, true for some speciic objects and relationships.

- (3) Find an algorithm to determine given some sentences of first order logic
regarded as premises and another sentence, being a desired conclusion, whether
that conclusion is provable from the premises using the rules of proof for first
order logic.
