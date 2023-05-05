Download Link: https://assignmentchef.com/product/solved-ece302-project-1-analytical-results
<br>
Accompanying code can be found on GitHub.

Let Xi be the random variable denoting the roll of a single die; let Yj = X1 + X2 + X3 be the random variable denoting the roll of three die to generate an ability score; let Z = max(Y1,Y2,Y3) be the random variable denoting the maximum of three trials to generate an ability score (using the “fun” method). All Xi are independent uniform IID; thus all Yj are independent uniform IID, and all Zk are independent uniform IID.

1.       (a) Three Bernoulli trials

(b)    Complement of a binomial distribution

(c)    Each trait is a Bernoulli trial

P(Zi = 18, 1 ≤ i ≤ 6) = (P(Z = 18))6

(d)   Get the set where all sums are ≤ 9, but at least one is equal to 9

P(Z = 9) = P(all sums ≤ 9) − P((all sums ≤ 9) ∧ (no sums = 9))

P(Zi = 9, 1 ≤ i ≤ 6) = (P(Z = 9))6

2.       Let Xi denote the random variable representing the hitpoints (hp) of a goblin, and Yj denote the random variable representing the damage (dmg) of a fireball shot. Note that Xi ∪ Yj are mutually independent.

(a)    Normal expected value

(b)    We can enumerate the pmf by inspection

P(X = 1) = P(X = 2) = P(X = 3) = P(X = 4) = 0.25

P(Y = 2) = P(Y = 4) = 0.25 P(Y = 3) = 0.5

(c)    We break up this question using a partition of Y .

P(slay all 6) =

(d)   We can break down the event in question into a partition of threeevents (note that it is not possible that the surviving troll has ≤ 2 hp or that the firebolt did 4 dmg):

i.        hp of surviving troll = 4, dmg = 3, all other trolls have hp ≤ 3

ii.      hp of surviving troll = 4, dmg = 2, all other trolls have hp ≤ 2

iii.    hp of surviving troll = 3, dmg = 2, all other trolls have hp ≤ 2

The probabilities of these events are easy to calculate.

Using Bayes’ rule, we can calculate the posterior pmf of X given that five trolls didn’t survive. Let W denote the event that the other five trolls died, and W = (i) ∪ (ii) ∪ (iii) ⇒ P(W) = P((i)) + P((ii)) + P((iii)) (union becomes addition since the events are disjoint). Then:

This in turn can be used to calculate the expected hp of the surviving troll:

(e) Let Zi denote the random variable denoting a roll of the 20-sided die (to decide whether Shedjam can hit Keene or not), Wj denote a roll of the 6-sided die (the Sword of Tuition’s damage), and Vk denote a roll of the 4-sided die (the Hammer of Tenure Denial’s damage).

E[dmg] = E[dmgSoT + dmgHTD]

= P(hitSoT)E[dmgSoT|hitSoT] + P(hitHTD)E[dmgHTD|hitHTD]