Download Link: https://assignmentchef.com/product/solved-cse310-homework-5
<br>
<strong><em>Q1) (40 points)</em></strong> Suppose you are implementing a dynamic set of student records as a hash table. Each record has an integer key.  Key can have values from 0 through 65,536 and no two records can have the same key values.  In addition to the key, each record has following information.

Name:

GPA:

Academic level:




Even though the key can take a value between 0 and 65536, this university can have max 10000 students at a given time.




Hash Table Implementation Details:

Assume that the hash key is <strong><u>k mod m and using chaining</u></strong> in case of a collision. The size (m) of the hash table (T) is 1000. Also, you can assume that keys for student are generated using a random uniform distribution function and each key is unique.




Write a C or C++ program that Implements the hash table construction for the above scenario and then implement the following three functions

<ol>

 <li>INSERT(T, x) // insert the student record x to the table</li>

 <li>DELETE(T, x) // delete the student record x from the table</li>

 <li>SEARCH(T, k) //search key k in the hash table</li>

</ol>













<strong>Q.2 [20 Pts]</strong> Graph Representation: Consider the following graph G and answer questions given below.







<ol>

 <li>[10 Points] Represent the above graph using adj-matrix and adj-list techniques.</li>

</ol>

<strong> </strong>

<ol>

 <li>[<em>10 Points] </em>The following table shows all the graph algorithms that we have discussed in the class. Fill the second and third column indicating running time and the space requirement for each algorithm</li>

</ol>

<table width="516">

 <tbody>

  <tr>

   <td width="144">Algorithm</td>

   <td width="204">Running Time</td>

   <td width="168">Space Requirements</td>

  </tr>

  <tr>

   <td width="144">BFS</td>

   <td width="204"> </td>

   <td width="168"> </td>

  </tr>

  <tr>

   <td width="144">DFS</td>

   <td width="204"> </td>

   <td width="168"> </td>

  </tr>

  <tr>

   <td width="144">Prim’s</td>

   <td width="204"> </td>

   <td width="168"> </td>

  </tr>

  <tr>

   <td width="144">Kruska’s</td>

   <td width="204"> </td>

   <td width="168"> </td>

  </tr>

  <tr>

   <td width="144">Dijkstra</td>

   <td width="204"> </td>

   <td width="168"> </td>

  </tr>

  <tr>

   <td width="144">Bellman-Ford</td>

   <td width="204"> </td>

   <td width="168"> </td>

  </tr>

 </tbody>

</table>







<ol start="3">

 <li><strong>(<em>15 points</em></strong>) Consider the graph G given below. Compute an MST of G using Prim’s algorithm. Specifically, list the edges selected into the tree in the correct order, and then draw the final MST. Must show all the intermediate steps for full credit</li>

</ol>




<ol start="4">

 <li><strong>(<em>15 points</em></strong>) Consider the graph G given in Problem 3 above. Compute an MST of G using Kruskal’s algorithm. Specifically, list the edges selected into the tree in the correct order, and draw the final MST. (You are encouraged to include all intermediate work, such as the results after doing each UNION operation, so that you can still receive partial credit if your final answer is incorrect.)</li>

 <li><strong><em>(20 Points)</em></strong> Consider the following Dijkstra’s algorithm discussed in the class and answer questions given below</li>

</ol>

DIJKSTRA(G, w, s)                 //G<u>:</u> directed with nonnegative edge weights      INIT-SINGLE-SOURCE(G, <em>s</em>)

S = Ø

Q = G.V                 // Q is a priority queue which we

// initialize with all the nodes in V[G]

<u>while</u> Q is not empty <u>do</u>

<em>u</em> = EXTRACT-MIN(Q)                      S = S  {<em>u</em>}

<u>for</u> each <em>v</em>  Adj[<em>u</em>] <u>do</u>

RELAX(<em>u</em>, <em>v</em>, w




<ol>

 <li>Use the algorithm above to find the shortest path from <strong><u>vertex 5</u></strong> to all other vertices in the graph given below as using adjacency matrix. First draw the graph for the given matrix and the show each step clearly in finding the shortest path. Value 0 indicate that there is no direct path.</li>

</ol>







1     2        3    4     5      6




<table width="203">

 <tbody>

  <tr>

   <td width="29"></td>

   <td width="174">


    <table width="168">

     <tbody>

      <tr>

       <td width="29">0</td>

       <td width="28">0</td>

       <td width="28">5</td>

       <td width="28">0</td>

       <td width="29">6</td>

       <td width="28">0</td>

      </tr>

      <tr>

       <td width="29">3</td>

       <td width="28">0</td>

       <td width="28">0</td>

       <td width="28">0</td>

       <td width="29">14</td>

       <td width="28">0</td>

      </tr>

      <tr>

       <td width="29">0</td>

       <td width="28">0</td>

       <td width="28">0</td>

       <td width="28">4</td>

       <td width="29">0</td>

       <td width="28">0</td>

      </tr>

      <tr>

       <td width="29">0</td>

       <td width="28">8</td>

       <td width="28">0</td>

       <td width="28">0</td>

       <td width="29">0</td>

       <td width="28">0</td>

      </tr>

      <tr>

       <td width="29">12</td>

       <td width="28">0</td>

       <td width="28">6</td>

       <td width="28">0</td>

       <td width="29">0</td>

       <td width="28">4</td>

      </tr>

      <tr>

       <td width="29">2</td>

       <td width="28">0</td>

       <td width="28">9</td>

       <td width="28">7</td>

       <td width="29">0</td>

       <td width="28">0</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>







<ol>

 <li>Now modify the Dijkstra’s so that it finds not only shortest paths, but also the compute the length of shortest paths and store them in a suitable data structure. Your data structure should return the shortest path distance from the source to any given node in O(1) time.</li>

 <li>Can we use Dijkstra’s algorithm to find the shortest paths in a graph with negative edges? Explain your answer clearly.</li>

</ol>







<strong><u>SUBMISSION INSTRUCTIONS</u> </strong>

Your C or C++ program for question 1  under the HW5 Q1 submission link a single PDF document with solutions to Questions 2- 5 under HW5 Q2-5 submission link


