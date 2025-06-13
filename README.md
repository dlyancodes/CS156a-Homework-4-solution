# CS156a-Homework-4-solution

Download Here: [CS156a Homework # 4 solution](https://jarviscodinghub.com/assignment/cs156a-homework-4-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

Definitions and notation follow the lectures. All questions have multiple-choice answers ([a], [b], [c], …). Collaboration is allowed but without discussing selected or
excluded choices. Your solutions must be based on your own work. See the initial
“Course Description and Policies” handout for important details about collaboration and “open book” policies.
Note about the homework
• Answer each question by deriving the answer (carries 6 points) then selecting
from the multiple-choice answers (carries 4 points). You can select 1 or 2 of
the multiple-choice answers for each question, but you will get 4 or 2 points,
respectively, for a correct answer. See the initial “Course Description and
Policies” handout for important details.
• The problems range from easy to difficult, and from practical to theoretical.
Some problems require running a full experiment to arrive at the answer.
• The answer may not be obvious or numerically close to one of the choices,
but one (and only one) choice will be correct if you follow the instructions
precisely in each problem. You are encouraged to explore the problem further
by experimenting with variations on these instructions, for the learning benefit.
• You are encouraged to take part in the discussion forum. Please make sure you
don’t discuss specific answers, or specific excluded answers, before the homework
is due.
c 2012-2018 Yaser Abu-Mostafa. All rights reserved. No redistribution in any
format. No translation or derivative products without written permission.
1
• Generalization Error
In Problems 1-3, we look at generalization bounds numerically. For N > dvc, use the
simple approximate bound Ndvc for the growth function mH(N).
1. For an H with dvc = 10, if you want 95% confidence that your generalization
error is at most 0.05, what is the closest numerical approximation of the sample
size that the VC generalization bound predicts?
[a] 400,000
[b] 420,000
[c] 440,000
[d] 460,000
[e] 480,000
2. There are a number of bounds on the generalization error , all holding with
probability at least 1−δ. Fix dvc = 50 and δ = 0.05 and plot these bounds as a
function of N. Which bound is the smallest for very large N, say N = 10, 000?
Note that [c] and [d] are implicit bounds in .
[a] Original VC bound:  ≤
q
8
N
ln 4mH(2N)
δ
[b] Rademacher Penalty Bound:  ≤
q2 ln(2NmH(N))
N +
q
2
N
ln 1
δ +
1
N
[c] Parrondo and Van den Broek:  ≤
q
1
N
(2 + ln 6mH(2N)
δ
)
[d] Devroye:  ≤
q
1
2N
(4(1 + ) + ln 4mH(N2)
δ
)
[e] They are all equal.
3. For the same values of dvc and δ of Problem 2, but for small N, say N = 5,
which bound is the smallest?
[a] Original VC bound:  ≤
q
8
N
ln 4mH(2N)
δ
[b] Rademacher Penalty Bound:  ≤
q2 ln(2NmH(N))
N +
q
2
N
ln 1
δ +
1
N
[c] Parrondo and Van den Broek:  ≤
q
1
N
(2 + ln 6mH(2N)
δ
)
[d] Devroye:  ≤
q
1
2N
(4(1 + ) + ln 4mH(N2)
δ
)
[e] They are all equal.
2
• Bias and Variance
Consider the case where the target function f : [−1, 1] → R is given by f(x) = sin(πx)
and the input probability distribution is uniform on [−1, 1]. Assume that the training
set has only two examples (picked independently), and that the learning algorithm
produces the hypothesis that minimizes the mean squared error on the examples.
4. Assume the learning model consists of all hypotheses of the form h(x) = ax.
What is the expected value, ¯g(x), of the hypothesis produced by the learning
algorithm (expected value with respect to the data set)? Express your ¯g(x) as
axˆ , and round ˆa to two decimal digits only, then match exactly to one of the
following answers.
[a] g¯(x) = 0
[b] g¯(x) = 0.79x
[c] g¯(x) = 1.07x
[d] g¯(x) = 1.58x
[e] None of the above
5. What is the closest value to the bias in this case?
[a] 0.1
[b] 0.3
[c] 0.5
[d] 0.7
[e] 1.0
6. What is the closest value to the variance in this case?
[a] 0.2
[b] 0.4
[c] 0.6
[d] 0.8
[e] 1.0
7. Now, let’s change H. Which of the following learning models has the least
expected value of out-of-sample error?
[a] Hypotheses of the form h(x) = b
[b] Hypotheses of the form h(x) = ax
3
[c] Hypotheses of the form h(x) = ax + b
[d] Hypotheses of the form h(x) = ax2
[e] Hypotheses of the form h(x) = ax2 + b
• VC Dimension
8. Let q ≥ 1 be an integer, and assume that mH(1) = 2. What is the VC dimension
of a hypothesis set whose growth function for all N ≥ 1 satisfies: mH(N + 1) =
2mH(N) −
N
q

? Recall that M
m

= 0 when m > M.
[a] q − 2
[b] q − 1
[c] q
[d] q + 1
[e] None of the above
9. For hypothesis sets H1, H2, …, HK with finite, positive VC dimensions dvc(Hk)
(same input space X ), some of the following bounds are correct and some are
not. Which, among the correct ones, is the tightest bound (the smallest range
of values) on the VC dimension of the intersection of the sets: dvc(
TK
k=1Hk)?
(The VC dimension of an empty set or a singleton set is taken as zero)
[a] 0 ≤ dvc(
TK
k=1Hk) ≤
PK
k=1 dvc(Hk)
[b] 0 ≤ dvc(
TK
k=1Hk) ≤ min{dvc(Hk)}
K
k=1
[c] 0 ≤ dvc(
TK
k=1Hk) ≤ max{dvc(Hk)}
K
k=1
[d] min{dvc(Hk)}
K
k=1 ≤ dvc(
TK
k=1Hk) ≤ max{dvc(Hk)}
K
k=1
[e] min{dvc(Hk)}
K
k=1 ≤ dvc(
TK
k=1Hk) ≤
PK
k=1 dvc(Hk)
10. For hypothesis sets H1, H2, …, HK with finite, positive VC dimensions dvc(Hk)
(same input space X ), some of the following bounds are correct and some are
not. Which, among the correct ones, is the tightest bound (the smallest range
of values) on the VC dimension of the union of the sets: dvc(
SK
k=1Hk)?
[a] 0 ≤ dvc(
SK
k=1Hk) ≤
PK
k=1 dvc(Hk)
[b] 0 ≤ dvc(
SK
k=1Hk) ≤ K − 1 + PK
k=1 dvc(Hk)
[c] min{dvc(Hk)}
K
k=1 ≤ dvc(
SK
k=1Hk) ≤
PK
k=1 dvc(Hk)
[d] max{dvc(Hk)}
K
k=1 ≤ dvc(
SK
k=1Hk) ≤
PK
k=1 dvc(Hk)
[e] max{dvc(Hk)}
K
k=1 ≤ dvc(
SK
k=1Hk) ≤ K − 1 + PK
k=1 dvc(Hk)

