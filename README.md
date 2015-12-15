# Practice 2015 - 06: Arrow Addition

## Background
Hawkeye is trying to bring down the Chitauri, but he doesn’t have enough arrows
to hit all of them. He knows how much damage each arrow will do to an enemy,
and he knows how much health each one has.

He doesn’t want to waste arrows, so he does not want to cause more damage than
an enemy has health. For any given Chitauri, he can choose from a large number
of arrow combinations to do enough damage to bring it down. Obviously, the
number of ways to reach this target damage is dependent on the available arrows.
For example, there are four ways to reach exactly 10 points of damage using arrows
that cause 1, 5, and 10 points of damage respectively. There are more ways to do
more than 10 points of damage, but we are not considering cases of causing more
than 10 points of damage for this problem. However, if we also allow an arrow
that does 2 points of damage, then there are now eleven ways to reach 10 points
of damage. The order in which he shoots the arrows does not matter.

Hawkeye wants to write a program that determines the number of possible ways to
bring down a Chitauri given its health and the types of arrows available to him.

## Description

### Input
The first line of the file will have an integer, n, which is the number of test
cases in this file. Each test case comprises three lines. The first line
contains two integers, s and t, which represent the number of distinct arrow
types and the number of target health amounts, respectively. The second line
contains s integers v(1), v(2), ..., v(s) which provide the values of each arrow
type in ascending order. These values are space separated. You are always
guaranteed v 1 = 1, which ensures that you can reach any health amount. The
third line contains t integers x(1), x(2), ..., x(t) which provide the target
health amounts. These values are also space separated.

In the first example below, the input file has 2 test cases: the first has
arrows of value 1, 5, 10, 25, and asks for the number of ways to reach 10
health points 50 health points. The second test case uses a base-2 system
with arrows of value 1, 2, 4, 8, and 16; it asks for the number of ways to
reach 10, 50, and 63 health points.

All given arrow types will have a value between 1 and 50. All health ranges
will be between 1 and 150.

### Output

## Sample
### Input
```
2
4 2
1 5 10 25
10 50
5 3
1 2 4 8 16
10 50 63
```

### Output
```
Case 1: 4 49
Case 2: 14 740 1460
```
