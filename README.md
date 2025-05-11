# Graph Representations

Implement a function that converts an adjacency matrix to an adjacency list for
a directed unweighted graph using the template in `code.js`. Test your new
function; I've provided some basic testing code that uses
[jsverify](https://jsverify.github.io/) in `code.test.js`. Now, the test code
does contain the solution, so you can have a look at it if you get stuck, but
try not to peek before attempting to solve it on your own.

## Runtime Analysis

What is the runtime complexity of the conversion that you implemented? Does it
depend on the number of vertices, the number of edges, or both?

Describe your reasoning and the conclusion you've come to. Your reasoning is the
most important part. Add your answer to this markdown file.

## Bonus

Implement a function to convert an adjacency list to an adjacency matrix and
analyze it as above.

Runtime (matrix to list):
Iterate over each vertex (row in matrix): $\Theta$(V)
For each vertex, iterate over all possible destinations: $\Theta$(V)
Check if there is an edge: $\Theta$(1)
Add edge to adjacency list if it exists: $\Theta$(1)
Total work: $\Theta$(V*V) = $\Theta$(V^2)

To determine the runtime of converting an adjanecy matrix to an adjacency list, the number of vertices (V) in the graph must be considered. The adjacency matrix for a graph with (V) vertices has (V*V) entries, regardless of the amount of edges. To perform the conversion, we must evaluate each entry in this matrix to see if an edge exists from vertex (i) to vertex (j). This requires the scanning of every row and column, resulting in a total of V^2 operations. Therefore, the runtime complexity of converting an adjacency matrix to an adjaceny list has a runtime complexity of $\Theta$(V^2), which is dependent only on the number of vertices.


“I certify that I have listed all sources used to complete this exercise, including the use
of any Large Language Models. All of the work is my own, except where stated
otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is
suspected, charges may be filed against me without prior notice.”

For this assignment, I asked Chat GPT for help articulating the reasoning for my conclusion.