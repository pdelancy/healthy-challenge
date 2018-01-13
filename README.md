# healthy-challenge

This is a simple app that finds the Levenshtein Distance between two strings, with a twist. In this project, I find the 
distance between two strings under the conditions that 1) I may only perform the following operations: add a letter, subtract a
letter, exchange a letter, or rearrange the string and 2) every intermediate string must also be a word. In addition, the 
user may assign the respective "costs" of each operation. This program finds the path between two words that has the least 
"cost".

To accomplish this, I convert a list of words into a graph, and I then implement a breadth first search of the graph to
traverse from the starting word to the end word. Throughout, I keep track of the cost of each path, and if the current path
exceeds the cost of a previously completed path, I curtail the pursuit of the current path.

To use this application, simply clone the repo and open the html file in your preferred web browser. You may also follow this
link: file:///Users/pdelancy1/Coding_Challenges/Rally_Health/RallyHealth.html.
