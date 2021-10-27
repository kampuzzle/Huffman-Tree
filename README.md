# Huffman-Tree
This is a WinRAR-like program developed in my second year of college using binary trees and lists. In this project we were asked to develop a program that would read an file 
and zip/unzip it based on the Huffman encoding. 

The idea of it was that, receiving in the terminal both the word for compacting/descompacting and the name of the file, the program should create another file with .comp
temination, if the word received in the terminal was Compacta, and creace an file with the original termination if the word was Descompacta.

---
### The Huffman Encoding
This cryptography system creates a binary tree based on how often a character appears in a file. The more often it appears, higher will be the position of the character in the 
binary tree. After creating the tree, the values (in the ASCII table) of each character will be replaced by another value, determined by the position of the character in the tree.
If the character is closer to the top of the tree (i.e appears very often in the file), it's new value will be smaller. If it is closer to the bottom of the tree (i.e appears 
rarely in the file), the value will be bigger. 

---
### Preparations
In the first steps to this project, we created a code to read a file and sort the characters of it based on how often it appeared in the file. After this, we made a binary tree
storing the characters and a table to relate the characters with it's new values based in the position of it in the tree. Everytime we access a right branch we add a 1 to the
binary number representing the character and everytime we access a left branch, we add a 0.

---
### Compacta
