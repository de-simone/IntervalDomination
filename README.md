# Pick the Closest Number Game

**Numerical solution to the following puzzle**

Three players A, B, C play the following game. First, A picks a real number in `[0,1]`, 
then B picks a number in the same range (different from A’s choice) and finally C picks a number, 
also in the same range, (different from the two chosen numbers). We then pick a random number `x` in `[0,1]` with uniform distribution. 
Whoever’s number is closest to `x` wins the game. Assume that A, B and C all play optimally and their sole goal is to maximise their chances of winning. 
Also assume that if one of them has several optimal choices, then that player will randomly pick one of the optimal choices.

1. If A chooses 0, then what is the best choice for B?
2. What is the best choice for A?
3. Can you write a program to figure out the best choice for the first player when the game is played among four players?

The questions above can be solved analytically, resulting into:

1. `b=2/3`
2. `a=1/4, a=3/4`
3. `a=1/5, a=4/5`

where `a` and `b` are the numbers chosen by players A and B, respectively. 

The code provided as a Jupyter notebook addresses numerically all of the questions above.

The solution strategy of this sequential game is by **backward induction**.
