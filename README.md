# implementing-binary-search-tree
Assignment: Implementing Binary Tree
Operations
Introduction
Imagine we are software engineers tasked with developing a binary tree management system for a
university database application. This system needs to handle various operations such as search,
insert, update, and delete efficiently for student records.
Starter Files
Start with a new Jupyter Notebook.
Dataset
Here is the dataset representing student records that we will use to populate the binary trees:
dataset = [(1, "Alice"), (2, "Bob"), (3, "Charlie"), (4, "David"), (5,
"Eve"), (6, "Frank"), (7, "Grace")]
Requirements
Define Classes and Constructors:
Create a TreeNode class to represent each node in the tree.
Create a BinaryTree class to manage the binary tree operations.
Implement Core Operations:
Implement the following operations in the BinaryTree class:
search(student_id): Search for a node with the given student ID.
insert(student_id, name): Insert a new node with the given student ID and name.
update(student_id, new_name): Update the name of an existing node.
delete(student_id): Delete a node with the given student ID.
Create Different Types of Binary Trees:
Implement methods to create the following types of binary trees:
Full Binary Tree
Complete Binary Tree
Degenerate (Pathological) Tree
Skewed Binary Tree
Interactive Component:
Implement an interactive menu allowing us to perform operations and view results
dynamically.
Pseudo-code Instructions:
1. Define the TreeNode Class:
Create a class called TreeNode.
Define the __init__ method to initialize student_id, name, left, and right
attributes.
Pseudo-code for TreeNode Class:
class TreeNode:
- Initialize the class with student_id, name, left child, and right
child attributes.
2. Define the BinaryTree Class:
Create a class called BinaryTree.
Define the __init__ method to initialize the root of the tree.
Implement the core operations: search, insert, update, delete.
Implement methods to create different types of binary trees.
Implement a method to print the tree for verification.
Pseudo-code for BinaryTree Class:
class BinaryTree:
- Initialize the class with an empty root and an empty list for values.
- Define methods for core operations: search, insert, update, delete.
- Define methods to create full, complete, degenerate, and skewed
binary trees.
- Define a method to print the tree for verification.
3. Implement Core Operations:
Implement the search method to locate a node within the tree.
Implement the insert method to add a new node to the tree.
Implement the update method to modify the name of an existing node.
Implement the delete method to remove a node from the tree.
Pseudo-code for Core Operations:
# Search Operation
Define search function:
- If node is empty or matches student_id, return node.
- Recursively search in both left and right subtrees.
# Insert Operation
Define insert function:
- If root is empty, create new root node with student_id and name.
- Else, use helper function to recursively insert in left or right
subtree based on availability.
Define _insert_recursive helper function:
- If left child is empty, insert new node as left child.
- Else if right child is empty, insert new node as right child.
- Else, recursively call helper function on left subtree.
# Update Operation
Define update function:
- Search for node with student_id.
- If node found, update name to new_name.
# Delete Operation
Define delete function:
- Use helper function to recursively delete node in left or right
subtree.
- Return updated root.
Define _delete_recursive helper function:
- If node is empty, return node.
- If node matches student_id:
- Handle cases for leaf, single child, and two children.
- Return updated node and deleted node.
- Recursively call helper function on left or right subtree.
- Return updated node and deleted node.
Define _find_min helper function:
- Traverse left subtree to find and return the node with the smallest
value.
4. Create Different Types of Binary Trees:
Implement methods to create full, complete, degenerate, and skewed binary trees
using the provided dataset.
Pseudo-code for Creating Binary Trees:
# Full Binary Tree
Define create_full_binary_tree function:
- Insert nodes in this order: [(1, "Alice"), (2, "Bob"), (3, "Charlie"),
(4, "David"), (5, "Eve"), (6, "Frank"), (7, "Grace")]
- Ensure the structure is a full binary tree.
- Store initial values in values list.
# Complete Binary Tree
Define create_complete_binary_tree function:
- Insert nodes in this order: [(1, "Alice"), (2, "Bob"), (3, "Charlie"),
(4, "David"), (5, "Eve"), (6, "Frank")]
- Ensure the structure is a complete binary tree.
- Store initial values in values list.
# Degenerate Tree
Define create_degenerate_tree function:
- Insert nodes in this order: [(1, "Alice"), (2, "Bob"), (3, "Charlie"),
(4, "David"), (5, "Eve")]
- Ensure the structure is a degenerate tree.
- Store initial values in values list.
# Skewed Tree
Define create_skewed_binary_tree function:
- Insert nodes in this order: [(1, "Alice"), (2, "Bob"), (3, "Charlie"),
(4, "David"), (5, "Eve")]
- Ensure the structure is a skewed tree.
- Store initial values in values list.
5. Interactive Component:
Implement an interactive menu allowing us to perform operations and view results
dynamically.
Pseudo-code for Interactive Menu:
Define display_tree_menu function:
- Print options for selecting a tree.
Define display_operation_menu function:
- Print current tree name and initial values.
- Print options for performing operations.
Define main function:
- Initialize different types of binary trees and store them in a
dictionary.
- Loop to display tree selection menu and operation menu.
- Based on user input, perform the selected operation on the chosen tree.
Expected Output:
Dataset: [(1, "Alice"), (2, "Bob"), (3, "Charlie"), (4, "David"), (5,
"Eve"), (6, "Frank"), (7, "Grace")]
Select a Tree:
1. Full Binary Tree
2. Complete Binary Tree
3. Degenerate Binary Tree
4. Skewed Binary Tree
5. Exit
Select a tree:
Binary Tree Operations Menu (Full Binary Tree)
Initial values in the tree: [(1, "Alice"), (2, "Bob"), (3, "Charlie"), (4,
"David"), (5, "Eve"), (6, "Frank"), (7, "Grace")]
1. Insert Node
2. Search for Node
3. Update Node Name
4. Delete Node
5. Back to Tree Selection
Select an operation:
