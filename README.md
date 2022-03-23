# Exploring The Idea of Turing Completeness

### The Entscheidungs Problem
-The problem to decide for every statement in first-order logic whether or not it is derivable in that logic.

Note that in its original form (Hilbert & Ackermann 1928), the problem was stated in terms of validity rather than derivability. Given Gödel’s completeness theorem (Gödel 1929) proving that there is an effective procedure (or not) for derivability is also a solution to the problem in its validity form. In order to tackle this problem, one needs a formalized notion of “effective procedure” and Turing’s machines were intended to do exactly that.

may be stated in the following three equivalent ways:

- (1) Find an algorithm to determine whether a given sentence of first order logic
is valid, that is, true regardless of what specific objects and relationships are
being reasoned about.

- (2) Find an algorithm to determine whether a given sentence of first order logic
is satisiable, that is, true for some speciic objects and relationships.

- (3) Find an algorithm to determine given some sentences of first order logic
regarded as premises and another sentence, being a desired conclusion, whether
that conclusion is provable from the premises using the rules of proof for first
order logic.

If we think of the premises as the axioms of some mathematical domain, we can
see that an actual algorithm solving the Entscheidungsproblem would reduce all
of mathematics, at least in principle, to mechanical calculation. Presumably it was
this that led Hilbert to characterise the Entscheidungsproblem as ‘the fundamental
problem of mathematical logic’.

### Turing Machines

Turing introduced Turing machines in the context of research into the foundations of mathematics. More particularly, he used these abstract devices to prove that there is no effective general method or procedure to solve, calculate or compute every instance of the Entscheidungs problem.

A Turing machine then, or a computing machine as Turing called it, in Turing’s original definition is a machine capable of a finite set of configurations: *q<sub>1</sub>, ..., q<sub>n</sub>*

It is supplied with a one-way infinite and one-dimensional tape divided into squares each capable of carrying exactly one symbol. At any moment, the machine is scanning the content of square *r* which is either bank (*S<sub>0</sub>*) or contains a symbol *S<sub>1</sub>, ..., S<sub>m</sub>* 
with *S<sub>1</sub>* = 0 and *S<sub>2</sub>* = 1.

There are two important things to notice about the Turing machine setup. The first concerns the definition of the machine itself, namely that the machine’s tape is potentially infinite. This corresponds to an assumption that the memory of the machine is (potentially) infinite. The second concerns the definition of Turing computable, namely that a function will be Turing computable if there exists a set of instructions that will result in a Turing machine computing the function regardless of the amount of time it takes.

If we moreover assume that a physical computer is a finite realization of the Turing machine, and so that the Turing machine functions as a good formal model for the computer, a result which shows that a function is not Turing computable is very strong, since it implies that no computer that we could ever build could carry out the computation.

### The Universal Turing Machine
The universal Turing machine which was constructed to prove the uncomputability of certain problems, is, roughly speaking, a Turing machine that is able to compute what any other Turing machine computes. Assuming that the Turing machine notion fully captures computability (and so that Turing’s thesis is valid), it is implied that anything which can be “computed”, can also be computed by that one universal machine. Conversely, any problem that is not computable by the universal machine is considered to be uncomputable.

This is the rhetorical and theoretical power of the universal machine concept, viz. that one relatively simple formal device captures all “the possible processes which can be carried out in computing a number” (Turing 1936–7). 

### Turing Completeness
A programming language is said to be Turing complete or computationally universal if it can be used to simulate arbitrary Turing machines.
