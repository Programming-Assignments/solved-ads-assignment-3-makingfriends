Download Link: https://assignmentchef.com/product/solved-ads-assignment-3-makingfriends
<br>
Your are a consultant of a recently started making-friend-agency. Soon you are planning to host an event where the goal is to help everyone befriend everyone else at the event. It is widely known that the friend of a friend automatically becomes your friend. Therefore it is only of importance to connect all people, once there is a friendly path (a path of friendships) between two people they will soon become friends.

Since you, as all consultants and more specifically all programmers, are lazy you want to minimize the effort you have to put in. Therefore all needed information about the participants have been collected and from this you can extract the compatability of two people. From this you have predicted how many minutes you would have to spend on introducing some pairs of people. Due to your laziness you have not predicted the number of minutes to introduce all pairs of people, only a subset of the pairs, however it is guaranteed that there is a path of predicted pairs between all pairs of people (i.e. it is possible to construct a path between each pair of people). Now the goal is to minimize your amount of work in order to connect all people.

<h1>Aims</h1>

The goals of the lab are:

<ul>

 <li>Implementing an algorithm to solve Minimal Spanning Tree. (Prim’s or Kruskal’s algorithms are recommended.)</li>

 <li>Debugging your code.</li>

 <li>Structuring your code in a logical fashion.</li>

 <li>Reason about correctness of your algorithm.</li>

 <li>Reason about upper bounds for time complexity.</li>

</ul>

<h1>Problem formulation</h1>

You are given a number of people and a number of undirected weighted edges between them (the weight being the number of minutes you would have to spend in order for the pair to become friends). The task is to print the number of minutes you will have to spend (in total) in order to connect all people.

<h1>Input</h1>

The first line of the input consists of two integers, <em>N,M</em>, the number of people at the event and the number of pairs for which you have predicted the time it would take you to make them friends. It is guaranteed that 2 ≤ <em>N </em>≤ 10<sup>5 </sup>and 1 ≤ <em>M </em>≤ min(<em>N </em>· (<em>N </em>− 1)<em>/</em>2<em>,</em>3 · 10<sup>6</sup>). Then follows <em>M </em>lines containing the description of each edge. Each of these lines contain three integers <em>u,v,w</em>, where 1 ≤ <em>u,v </em>≤ <em>N </em>are the indices of the persons of the edge and 0 ≤ <em>w </em>≤ 10<sup>6 </sup>is the weight of the edge, i.e. the number of minutes it would take you to make <em>u </em>and <em>v </em>friends. It is guaranteed that each pair {<em>u,v</em>} occurs at most once in the input.

<h1>Output</h1>

The output should contain a single integer on a single line, the total sum of the weights of the minimal spanning tree in the graph – i.e. the miminal total number of minutes you would have to spend on connecting all people.

<h1>Examination and Points of Discussion</h1>

To pass the lab make sure you have:

<ul>

 <li>Have successfully implemented the algorithm with the correct time complexity.</li>

 <li>Have neat and understandable code.</li>

 <li>Have descriptive variable names.</li>

 <li>Have filled in the blanks in the report.</li>

 <li>Have run the check_solution script to validate your solution.</li>

</ul>

During the oral presentation you will discuss the follwoing questions with the lab assistant:

<ul>

 <li>Why does the algorithm you have implemented produce a minimal spanning tree?</li>

 <li>What is the time complexity, and more importantly why?</li>

 <li>What happens if one of the edges you have chosen to include collapses? Might there be any problems with that in real applications?</li>

 <li>Can you think of any real applications of MST? What would the requirements of a problem need to be in order for us to want MST as a solution?</li>

</ul>

<strong>Sample Input 1                                                                                 Sample Output 1</strong>

<table width="622">

 <tbody>

  <tr>

   <td width="311">3 21     2 32     3 7</td>

   <td width="311">10</td>

  </tr>

 </tbody>

</table>

<strong>Sample Input 2                                                                                 Sample Output 2</strong>

<table width="622">

 <tbody>

  <tr>

   <td width="311">4 41     2 12     3 43     4 51 3 7</td>

   <td width="311">10</td>

  </tr>

 </tbody>

</table>


