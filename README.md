Download Link: https://assignmentchef.com/product/solved-eso207-data-structures-and-algorithms-theory-assignment-2
<br>









<h1>Part 1</h1>

<strong>Problem1</strong> Let <em>G </em>= (<em>V,E</em>) be any unweighted directed graph on |<em>V </em>| = <em>n </em>vertices and |<em>E</em>| = <em>m </em>edges with source <em>s </em>∈ <em>V </em>and destination <em>t </em>∈ <em>V </em>. Moreover <em>t </em>is reachable from <em>s</em>.

<em>G </em>is said to be <em>1-connected </em>if there exists a subset <em>E</em><sub>1 </sub>⊆ <em>E </em>such that if we remove any one edge <em>e </em>∈ <em>E</em><sub>1 </sub>then it partitions the vertex set <em>V </em>into two non empty subsets <em>S,T </em>such that there is no path from <em>s </em>∈ <em>S </em>to <em>t </em>∈ <em>T </em>in <em>G </em>= (<em>V,E </em> {<em>e</em>}).

Consider <em>G </em>to be a given <em>1-connected </em>unweighted directed graph. Preprocess <em>G </em>in <em>O</em>(<em>n </em>+ <em>m</em>) time and build a data structure of size <em>O</em>(<em>n </em>+ <em>m</em>) to answer the following 1<em>-connectivity </em>query in <em>O</em>(1) time,

(

1        if graph <em>G </em>is still <em>1-connected </em>after removing <em>e </em>∈ <em>E</em>

1-connectivity(<em>G,e</em>) =                                                                                                                                                      (1)

0    otherwise

Give pseudo code for preprocessing step and prove the time and space complexity. Also give the pseudocode and explain how a query, <em>1-connectivity</em>(<em>G,e</em>) is handled using the constructed data structure in <em>O</em>(1) time.

<strong>Problem2</strong>. An array <em>A </em>is given with <em>n </em>numbers. A pair (<em>i,j</em>) with 0 ≤ <em>i &lt; j &lt; n </em>is said to be <em>strongly dominated </em>if <em>A</em>[<em>i</em>] <em>&gt; </em>2<em>A</em>[<em>j</em>]. Design an <em>O</em>(<em>n</em>log<em>n</em>) time algorithm that reports the total number of <em>strongly dominated </em>pairs in <em>A </em>and prove the time complexity of your algorithm.

<strong>Problem3</strong>.  Let <em>P </em>= {<em>p</em><sub>1</sub><em>,p</em><sub>2</sub><em>,…,p<sub>n</sub></em>} be a set of <em>n </em>points given in 2<em>D </em>where <em>p<sub>i </sub></em>= (<em>x,y<sub>i</sub></em>) and <em>y<sub>i </sub></em>6= <em>y<sub>j </sub></em>for all <em>i </em>6= <em>j</em>. Additionally two more points <em>s </em>= (<em>x<sub>s</sub>,y<sub>s</sub></em>) and <em>t </em>= (<em>x<sub>t</sub>,y<sub>t</sub></em>) are given where <em>x<sub>s </sub>&lt; x </em>and <em>x<sub>t </sub>&gt; x</em>. A path between <em>s </em>and <em>t </em>must contain exactly one point <em>p<sub>i </sub></em>∈ <em>P</em>, (In other words, it is a path of length 2, <em>s </em>7→ <em>p<sub>i </sub></em>7→ <em>t</em>, where <em>p<sub>i </sub></em>∈ <em>P</em>). Cost of an edge is the Euclidean distance between the pair of points. Hence the cost of a path is the sum of distances of every edge in the path. Your task is to build a compact data structure in <em>O</em>(<em>n</em>log<em>n</em>) time and <em>O</em>(<em>n</em>) size that will be able to answer the following <em>Min-Cost-Point </em>query in <em>O</em>(log<em>n</em>) worst case time.

<em>Min-Cost-Point</em>(<em>P,s,t</em>) = { <em>p<sub>k </sub></em>| <em>p<sub>k </sub></em>∈ <em>P </em>and the cost of path between <em>s </em>and <em>t </em>including <em>p<sub>k </sub></em>is minimized.}.

Query outputs an appropriate point <em>p<sub>k </sub></em>from <em>P </em>such that the cost of the path between <em>s </em>and <em>t </em>including point <em>p<sub>k </sub></em>is minimized, for any given <em>s </em>and <em>t</em>.

Also you are not allowed to sort the points in <em>P</em>. Assume that computing distance between a pair of points takes <em>O</em>(1) time, further computing the cost of a 2-path takes time <em>O</em>(1).

Give the pseudo code for preprocessing step and prove the time and space complexity. You must also give pseudo code or explain how a query is handled using the constructed data structure in <em>O</em>(log<em>n</em>) time.

<h1>Part 2</h1>

<strong>Problem4</strong>. Given an array <em>A </em>of integers , you have to return an array <em>count </em>where each index <em>i</em>, the array <em>count</em>[<em>i</em>] is the number of smaller elements to the right of <em>A</em>[<em>i</em>].

Give <em>O</em>(<em>n</em>log<em>n</em>) runtime pseudo code to solve the above problem. Prove the time complexity of your algorithm.

<strong>Example :</strong>

Input: <em>A </em>= [5<em>,</em>2<em>,</em>6<em>,</em>1] Output: [2<em>,</em>1<em>,</em>1<em>,</em>0] Explanation:

To the right of 5 there are 2 smaller elements (2 and 1).

To the right of 2 there is only 1 smaller element (1).

To the right of 6 there is 1 smaller element (1). To the right of 1 there is 0 smaller element.

<strong>Problem5</strong>.Give an algorithm that determines whether or not a given undirected graph <em>G </em>= (<em>V,E</em>) contains a cycle. Your algorithm should run in <em>O</em>(<em>V </em>) time, independent of the number of edges in <em>G</em>. Mention the data structures used in the algorithm. Analyze the time complexity of your algorithm.

<strong>Problem6</strong>.A knight is a chess piece that moves in an L shape i.e the knight moves 2 units in one direction (i.e., horizontal or vertical) and 1 unit in the perpendicular direction. The figure below shows all the possible moves of knight from position (<em>e,</em>4).

You are given a square chess board of size <em>N </em>× <em>N</em>. The knight is initially at source point, (<em>C,D</em>) and destination point of the knight is (<em>E,F</em>). You need to find the minimum number of steps for the knight to move from source to destination. Note that the knight should not move out of the chess board at any point in time.

Give the pseudocode along with the analysis of time complexity and space complexity for the algorithm.

Example :

In the above example the knight takes 3 step to reach the target T i.e from (1,4) to (6,1). (1<em>,</em>4)− <em>&gt; </em>(4<em>,</em>5)− <em>&gt; </em>(5<em>,</em>3)− <em>&gt; </em>(6<em>,</em>1).