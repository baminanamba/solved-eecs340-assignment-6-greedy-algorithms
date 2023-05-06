Download Link: https://assignmentchef.com/product/solved-eecs340-assignment-6-greedy-algorithms
<br>
Problem 1

Prove that the following greedy choices do not lead to optimal solutions for the activity selection problem:

<ul>

 <li>Select the activity with the earliest starting time.</li>

 <li>Select the activity with least duration.</li>

 <li>Select the activity that overlaps the fewest other remaining activities.</li>

</ul>

<h1>Problem 2</h1>

We have <em>n </em>activities. Each activity requires <em>t<sub>i </sub></em>time to complete and has deadline <em>d<sub>i</sub></em>. We would like to schedule the activities to minimize the maximum delay in completing any activity; that is,

we would like to assign starting times <em>s<sub>i </sub></em>to all activities so that max<sub>1≤<em>i</em>≤<em>n</em></sub>{∆<em><sub>i</sub></em>} is minimized, where ∆<em><sub>i </sub></em>= <em>f<sub>i </sub></em>−<em>d<sub>i </sub></em>is the delay for activity <em>i </em>and <em>f<sub>i </sub></em>= <em>s<sub>i </sub></em>+<em>t<sub>i </sub></em>is the finishing time for activity <em>i</em>. Note that we can only perform one activity at a given time (if activity <em>i </em>starts at time <em>s<sub>i</sub></em>, the next scheduled activity has to start at time <em>f<sub>i</sub></em>).

For example, if <em>t </em>=<em>&lt; </em>10<em>,</em>5<em>,</em>6<em>,</em>2 <em>&gt; </em>and <em>d </em>=<em>&lt; </em>11<em>,</em>6<em>,</em>12<em>,</em>20 <em>&gt;</em>, then the optimal solution is to schedule the activities in the order <em>&lt; </em>2<em>,</em>1<em>,</em>3<em>,</em>4 <em>&gt; </em>to obtain starting/finishing times <em>s/f </em>=<em>&lt; </em>5<em>/</em>15<em>,</em>0<em>/</em>5<em>,</em>15<em>/</em>21<em>,</em>21<em>/</em>23 <em>&gt; </em>and achieve a maximum delay of 9 (for the third activity). State and prove the greedy choice property for this problem.

<h1>Problem 3</h1>

We have infinite supply of integer coin denominations of <em>c</em><sub>1 </sub>= 1 <em>&lt; c</em><sub>2 </sub><em>&lt; … &lt; c<sub>k </sub></em>to make change for a given an integer amount <em>n</em>. For this purpose, we would like to find the minimum number of coins that add up to <em>n</em>. An obvious greedy choice for this problem is to use the largest coin that has value less than or equal to <em>n </em>(e.g., if <em>c<sub>k </sub></em>≤ <em>n</em>, then return <em>c<sub>k</sub></em>, and solve the problem for <em>n </em>− <em>c<sub>k</sub></em>).

<ul>

 <li>Prove that, if the coin denominations are arbitrary, this greedy choice is not guaranteed to lead to an optimal solution.</li>

 <li>Prove that, if the coin denominations are powers of 2, i.e., <em>c<sub>i </sub></em>= 2<em><sup>i</sup></em><sup>−1 </sup>for 1 ≤ <em>i </em>≤ <em>k</em>, then this greedy choice is guaranteed to lead to an optimal solution.</li>

</ul>