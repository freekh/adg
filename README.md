# A Different Grammar (ADG)

The intent of project is internal research for the creation of a grammar of the shell language TAS (to be announced).
It is currently NOT READY.

It is a variation of todays most popular grammar specifications: PEG and BNF.

It is similiar to BNF because it features backtracking, but is unambigious as PEG.
In terms of operators it has the same ones as BNF, but has an ordered choice operator as PEG.

A bold (?) move is to use bloomfilters to increase performance/reduce footprint of BNF by using a bloom filter to detect
paths that have been traversed.

There is a chance of hash collisions, and this needs to be addressed before this grammar can be used.
