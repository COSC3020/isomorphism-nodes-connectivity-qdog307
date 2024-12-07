# Isomorphism

Prove that if two graphs $A$ and $B$ have the same number of nodes and are
completely connected, they must be isomorphic. I have started with the formal
definition of isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

### Proof

A complete graph with $n$ vertices has every pair of vertices connected by an edge. This means the number of edges in each graph is given by $|E| = \binom{n}{2} = \frac{n(n-1)}{2}$. Since $G_1$ and $G_2$ have the same number of vertices and are both completely connected, they also have the same number of edges.

Because the vertex sets of $G_1$ and $G_2$ have the same cardinality ($|V_1| = |V_2| = n$), we can define a bijection $f: V_1 \to V_2$. For any pair of vertices $(u, v) \in E_1$, their images under $f$, $(f(u), f(v))$, are connected in $G_2$ because every vertex in $G_2$ is connected to every other vertex. Similarly, because $f$ is bijective, for every edge $(f(u), f(v)) \in E_2$, the preimages $(u, v) \in E_1$. This ensures that adjacency relationships are preserved under $f$.

Since $f$ is a bijection that preserves adjacency relationships, and $G_1$ and $G_2$ have the same number of vertices and edges, $G_1$ and $G_2$ are isomorphic.

To define your $f$, we map each vertex in $V_1$ to a unique vertex in $V_2$. If the vertices of $V_1$ are labeled as $v_1, v_2, ..., v_n$ and the vertices of $V_2$ are labeled as $u_1, u_2, ..., u_n$, then $f(v_i) = u_i$ for all $i$.

This function $f$ is a bijection because it is one-to-one (no two vertices in $V_1$ map to the same vertex in $V_2$) and onto (every vertex in $V_2$ is the image of some vertex in $V_1$).


## Sources 

For this I looked through the lecture slides. I googled isomorphsim. I found these two websites to explain it a little better to me. I then watched this youtube to understand better. https://www.geeksforgeeks.org/complete-graph-in-graph-theory/ and https://youtu.be/EwV4Puk2coU?si=SFN5GU8fVPQUPlQx Finally I found a written paper that helped with the formal part. https://courses.grainger.illinois.edu/cs173/sp2010/Lectures/lect_32.pdf 

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.


