# tree_height_empty_py

Problem: Compute tree height
Problem Introduction
Trees are used to manipulate hierarchical data such as hierarchy of categories of a retailer or the directory
structure on your computer. They are also used in data analysis and machine learning both for hierarchical
clustering and building complex predictive models, including some of the best-performing in practice
algorithms like Gradient Boosting over Decision Trees and Random Forests. In the later modules of this
course, we will introduce balanced binary search trees (BST) — a special kind of trees that allows to very
efficiently store, manipulate and retrieve data. Balanced BSTs are thus used in databases for efficient storage
and actually in virtually any non-trivial programs, typically via built-in data structures of the programming
language at hand.
In this problem, your goal is to get used to trees. You will need to read a description of a tree from the
input, implement the tree data structure, store the tree and compute its height.
Problem Description
Task. You are given a description of a rooted tree. Your task is to compute and output its height. Recall
that the height of a (rooted) tree is the maximum depth of a node, or the maximum distance from a
leaf to the root. You are given an arbitrary tree, not necessarily a binary tree.
Input Format. The first line contains the number of nodes 𝑛. The second line contains 𝑛 integer numbers
from −1 to 𝑛 − 1 — parents of nodes. If the 𝑖-th one of them (0 ≤ 𝑖 ≤ 𝑛 − 1) is −1, node 𝑖 is the root,
otherwise it’s 0-based index of the parent of 𝑖-th node. It is guaranteed that there is exactly one root.
It is guaranteed that the input represents a tree.

Constraints. 1 ≤ 𝑛 ≤ 105.
Output Format. Output the height of the tree.

Memory Limit. 512MB.


# To pass the tests

implement input form keyboard and from files (capital i or capital F)

let user input file name to use, don't allow file names with letter a (don't forget that the files are located in a folder)
account for github input inprecision in both the file names and input




# Sample 1.
Input:
5
4 -1 4 1 1
Output:
3
The input means that there are 5 nodes with numbers from 0 to 4, node 0 is a child of node 4, node 1
is the root, node 2 is a child of node 4, node 3 is a child of node 1 and node 4 is a child of node 1. To
see this, let us write numbers of nodes from 0 to 4 in one line and the numbers given in the input in
the second line underneath:
0 1 2 3 4
4 -1 4 1 1
Now we can see that the node number 1 is the root, because −1 corresponds to it in the second line.
Also, we know that the nodes number 3 and number 4 are children of the root node 1. Also, we know
that the nodes number 0 and number 2 are children of the node 4.
The height of this tree is 3, because the number of vertices on the path from root 1 to leaf 2 is 3.
