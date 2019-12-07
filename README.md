# Sorular

İlk ünitedeki sorular.

Burada "Hint" dediği birtakım ipuçları:

1.1

Is Unique: Implement an algorithm to determine if a string has all unique characters. What if you cannot use additional data structures?

Hints: #44, #117, #732

1.2

Check Permutation: Given two strings,write a method to decide if one is a permutation of the other.

Hints: #7, #84, #722, #737

1.3

URLify: Write a method to replace all spaces in a string with '%20'. You may assume that the string has sufficient space at the end to hold the additional characters,and that you are given the "true" length of the string. (Note: If implementing in Java,please use a character array so that you can perform this operation in place.)

EXAMPLE

Input: "Mr John Smith ", 13 Output: "Mr%20John%20Smith" Hints: #53, #118

1.4

Palindrome Permutation: Given a string, write a function to check if it is a permutation of a palin­ drome. A palindrome is a word or phrase that is the same forwards and backwards. A permutation is a rearrangement of letters. The palindrome does not need to be limited to just dictionary words.

EXAMPLE

Input: Tact Coa

Output: True (permutations: "taco cat", "atco eta", etc.) Hints:#106,#121,#134,#136

1.5

One Away: There are three types of edits that can be performed on strings: insert a character, remove a character, or replace a character. Given two strings, write a function to check if they are one edit (or zero edits) away.

EXAMPLE

pale, ple -> true pales, pale -> true pale, bale -> true pale, bake -> false Hints:#23, #97, #130

1.6

String Compression: Implement a method to perform basic string compression using the counts of repeated characters. For example, the string aabcccccaaa would become a2blc5a3. If the "compressed" string would not become smaller than the original string, your method should return

the original string. You can assume the string has only uppercase and lowercase letters (a - z).

Hints:#92, #110

1.7

Rotate Matrix: Given an image represented by an NxN matrix, where each pixel in the image is 4 bytes, write a method to rotate the image by 90 degrees. Can you do this in place?

Hints:#51, #100

1.8

Zero Matrix: Write an algorithm such that if an element in an MxN matrix is 0, its entire row and column are set to 0.

Hints:#17, #74, #702

1.9

String Rotation: Assume you have a method isSubstring which checks if one word is a substring of another.

Given two strings, sl and s2, write code to check if s2 is a rotation of sl using only one call to isSubstring (e.g.,"waterbottle" is a rotation of"erbottlewat").

Hints:#34,#88, #704


@@@@@@@
2. Ünite soruları

NOT: Linked List nedir?

Tespih taneleri gibi, bir çizgide dizilmiş elemanlardan oluşan bir listedir. Burada önemli olan, bir elemanın, sadece kendisinden sonraki elemana dair bilgisi olmasıdır. Diğer elemanları bilmez.

Bunu yan yana dizilmiş kutular olarak düşünmek daha doğrudur. Her bir kutunun, sadece sağ tarafındaki diğer kutudan haberi var. Yani, sadece bir sonrakine geçiş yapılabilir.

2.1

Remove Dups!

Write code to remove duplicates from an unsorted linked list.

How would you solve this problem if a temporary buffer is not allowed?

Hints: #9, #40

(Sıralanmamış bir "Linked List" içindeki tekrar eden elemanları silmek.
Eğer bir "buffer" kullanılması yasak olsa idi, nasıl çözerdin?)

2.2

Return Kth to Last: Implement an algorithm to find the kth to last element of a singly linked list.

Hints:#8, #25, #41, #67, #126

(Bir "Linked List" içerisindeki en son elemana "bilmem kaçıncı" elemanı bulmak.

Burada "bilmem kaçıncı", "k'th" ile temsil edilmiş. Çünkü ingilizcede, birinci, ikinci, üçüncü gibi kelimelerin sonunca -nci, -nci eki "th" dir, yerine göre.

Bu yüzden k'th= k'nci eleman demek.

Yani sondan birinci, sondan ikinci elemanı bulmak gibi.)

2.3

Delete Middle Node: Implement an algorithm to delete a node in the middle (i.e., any node but the first and last node, not necessarily the exact middle) of a singly linked list, given only access to that node.

EXAMPLE

lnput:the node c from the linked list a->b->c->d->e->f

Result: nothing is returned, but the new linked list looks like a->b->d->e- >f

(Bir "Linked List"in, birinci ve sonuncu elemanı dışındaki herhangi bir elemanı silme. Sadece bu elemana erişim izni olacak.

ÖRNEK:

Şu listeden a->b->c->d->e->f ortadaki c elemanını silince a->b->d->e- >f sonucu elde etmek.

2.4

Partition: Write code to partition a linked list around a value x, such that all nodes less than x come before all nodes greater than or equal to x. If x is contained within the list, the values of x only need to be after the elements less than x (see below). The partition element x can appear anywhere in the "right partition"; it does not need to appear between the left and right partitions.

EXAMPLE

Input: 3 -> 5 -> 8 -> 5 -> 10 -> 2 -> 1[partition=5] Output: 3 -> 1 -> 2 -> 10 -> 5 -> 5 -> 8
Hints: #3, #24

Bir Linked List, içerisinde herhangi bir elemana göre, listeyi ikiye ayırmak. Örnekte 5 seçilmiş. 5'in solundakiler 5'ten küçük, sağındakiler ise 5'e eşit veya 5'ten büyük.

2.5

Sum Lists: You have two numbers represented by a linked list, where each node contains a single digit.The digits are stored in reverse order, such that the 1 's digit is at the head of the list. Write a function that adds the two numbers and returns the sum as a linked list.

EXAMPLE

Input:(7-> 1 -> 6) + (5 -> 9 -> 2).Thatis,617 + 295. Output:2 -> 1 -> 9.Thatis,912.
FOLLOW UP
Suppose the digits are stored in forward order. Repeat the above problem.

EXAMPLE

lnput:(6 -> 1 -> 7) + (2 -> 9 -> 5).

That is,617 + 295. Output:9 -> 1 -> 2.Thatis,912.
Hints: #7, #30, #71, #95, #109

Elinde iki tane sayı var. Ama bu sayı bir Linked List ile ifade edilmiş. "Ama tersten yazılmış. "

Yani sayıdaki her bir rakam, Linked List'in bir elemanı ile ifade ediliyor. Yani Link Listeki her bir elemanı bir kutu gibi düşünecek olursak, her bir kutuda, bir "rakam" olacak.

Bu iki rakamı toplayan bir fonksiyon yazman isteniyor.

İkinci örnekte ise, eğer tersten değil de, düzden yazılsa idi nasıl çözüleceğini soruyor.

2.6

Palindrome: Implement a function to check if a linked list is a palindrome. Hints:#5, #13, #29, #61, #101

(Bir Linked List ile ifade edilmiş kelimenin palindrome olup olmadığına bakın diyor)

2.7

Intersection: Given two (singly) linked lists, determine if the two lists intersect. Return the inter­ secting node. Note that the intersection is defined based on reference, not value.That is, if the kth node of the first linked list is the exact same node (by reference) as the jth node of the second linked list, then they are intersecting.

Hints:#20, #45, #55, #65, #76, #93, #111, #120, #129

(Verilen iki Linked List'in kesişip kesişmediğini bulun diyor. Mesela ilk listenin 5. elemanı ile, ikincisinin 5. elemanı aynı ise kesişiyor denir)

2.7
Loop Detection: Given a circular linked list, implement an algorithm that returns the node at the

beginning of the loop.

DEFINITION

Circular linked list: A (corrupt) linked list in which a node's next pointer points to an earlier node, so as to make a loop in the linked list.

EXAMPLE

Input: A -> B -> C -> D -> E -> C[the same Case earlier]

Output: C

Hints: #50, #69, #83, #90

Listede bir döngü olup olmadığını tespit edip, döngünün ilk elemanını bulun diyor.

Yukarıdaki örnekte, C dönmüş. Çünkü E tekrar C’ye bağlanarak bir döngü oluşturmuş. Yani bir kolye zincirinde, bir halkanın kendisinden önceki bir halkaya bağlanması gibi.
@@@@@@@
3. Ünite soruları:

Stack ve Queue ilgili.

Stack: Üst üste konulmuş tabaklar, üst üste konulmuş kitaplar. Ayrıca, Hanoi kuleleri de, en son elemanın en küçük olduğu türde bir stack örneğidir.

En büyük özelliği LIFO (Last in first out: Son giren ilk çıkar)

Queue: Kuyruk demektir. Her hangi bir fatura ödeme kuyruğuna benzetilebilir. En büyük özelliği FIFO (First in first out: İlk gelen ilk çıkar) olmasıdır.

3.1

Three in One: Describe how you could use a single array to implement three stacks. Hints: #2, #72, #38, #58

3.2

Stack Min: How would you design a stack which, in addition to push and pop, has a function min which returns the minimum element?

Push, pop and min should all operate in 0(1) time.

Hints:#27, #59, #78

3.3

Stack of Plates: Imagine a (literal) stack of plates. If the stack gets too high, it might topple.

composed of several stacks and should create a new stack once the previous one exceeds capacity. SetOfStacks. push() and SetOfStacks. pop() should behave identically to a single stack (that is, pop() should return the same values as it would if there were just a single stack).

FOLLOW UP

ImplementafunctionpopAt(int index)whichperformsapopoperationonaspecificsub-stack.

Hints:#64, #87

3.4

Queue via Stacks: Implement a MyQueue class which implements a queue using two stacks.

Hints: #98, #7 74

3.5

Sort Stack: Write a program to sort a stack such that the smallest items are on the top. You can use an additional temporary stack, but you may not copy the elements into any other data structure (such as an array). The stack supports the following operations: push, pop, peek, and isEmpty.

Hints:# 15, #32, #43

3.6

Animal Shelter: An animal shelter, which holds only dogs and cats, operates on a strictly"first in, first out" basis. People must adopt either the"oldest" (based on arrival time) of all animals at the shelter, or they can select whether they would prefer a dog or a cat (and will receive the oldest animal of that type). They cannot select which specific animal they would like. Create the data structures to maintain this system and implement operations such as enqueue, dequeueAny, dequeueDog, and dequeueCat. You may use the built-in Linked list data structure.

Hints:#22, #56, #63
@@@@@@@
4. Ünite soruları:

Tree ve Graph ile ilgili.

Tree: Ağaca benzeyen veri yapısı.

Graph: İnsan ilişkilerine benzeyen ve bu yüzden de sosyal medya algoritmalarında kullanılan veri yapısı. Her bir node'un diğer tüm node'larla iletişimi olabilir.

4.1

Route Between Nodes: Given a directed graph, design an algorithm to find out whether there is a route between two nodes.

Hints:#127

4.2

Minimal Tree: Given a sorted (increasing order) array with unique integer elements, write an algo­rithm to create a binary search tree with minimal height.

Hints:#79,#73,#776

4.3
List of Depths: Given a binary tree, design an algorithm which creates a linked list of all the nodes at each depth (e.g., if you have a tree with depth D, you'll have D linked lists).

Hints: #107, #123, #135

4.4

Check Balanced: Implement a function to check if a binary tree is balanced. For the purposes of this question, a balanced tree is defined to be a tree such that the heights of the two subtrees of any node never differ by more than one.

Hints:#27, #33, #49, #705, #724

4.5
Validate Binary Search Tree: Implement a function to check if a binary tree is a binary search tree.

Hints: #35, #57, #86, #113, #128

4.6

Successor: Write an algorithm to find the "next" node (i.e., in-order successor) of a given node in a binary search tree. You may assume that each node has a link to its parent.

Hints: #79, #91

4.7

Build Order: You are given a list of projects and a list of dependencies (which is a list of pairs of projects, where the second project is dependent on the first project). All of a project's dependencies must be built before the project is. Find a build order that will allow the projects to be built. If there is no valid build order, return an error.

EXAMPLE

Input:

projects: a, b, c, d, e, f

dependencies: (a, d), (f, b), (b, d), (f, a), (d, c) Output: f, e, a, b, d, c
Hints: #26, #47, #60, #85, #725, #133

4.8

First Common Ancestor: Design an algorithm and write code to find the first common ancestor of two nodes in a binary tree. Avoid storing additional nodes in a data structure. NOTE: This is not necessarily a binary search tree.

Hints: #70, #76, #28, #36, #46, #70, #80, #96

4.9

Binary Search Tree Sequences: A binary search tree was created by traversing through an array from left to right and inserting each element. Given a binary search tree with distinct elements, print all possible arrays that could have led to this tree.

EXAMPLE

Input:

Output: {2, 1, 3}, {2, 3, 1}

4.10

Check Subtree: T1 and T2 are two very large binary trees, with T1 much bigger than T2.

Create an algorithm to determine if T2 is a subtree of T1.

A tree T2 is a subtree of T1 if there exists a node n in T1 such that the subtree of n is identical to T2. That is, if you cut off the tree at node n, the two trees would be identical.

Hints:#4, #11, #18, #31, #37

4.11

Random Node: You are implementing a binary tree class from scratch which, in addition to insert, find, and delete, has a method getRandomNode() which returns a random node from the tree. All nodes should be equally likely to be chosen. Design and implement an algorithm for getRandomNode, and explain how you would implement the rest of the methods.

Hints: #42, #54, #62, #75, #89, #99, #112, #119

4.12

Paths with Sum: You are given a binary tree in which each node contains an integer value (which might be positive or negative). Design an algorithm to count the number of paths that sum to a given value. The path does not need to start or end at the root or a leaf, but it must go downwards (traveling only from parent nodes to child nodes).

Hints:#6, #14, #52, #68, #77, #87, #94, #103, #108, #115
@@@@@@@
5. ÜNİTE  Bit Manipülasyonu ile ilgili:

5.1: 

Insertion: You are given two 32-bit numbers, N and M, and two bit positions, i and j. Write a method to insert M into N such that M starts at bit j and ends at bit i. 

You can assume that the bits j through i have enough space to fit all of M. 

That is, if M = 10011, you can assume that there are at least 5 bits between j and i. You would not, for example, have j = 3 and i = 2, because M could not fully fit between bit 3 and bit 2.

EXAMPLE

Input: N 10000000000, M 10011, i 2, j 6 Output:N = 10001001100
 Hints: #137, #769, #215
 İki adet sayı var: M ve N.   N sayısını, M sayısının içine enjekte etmemiz isteniyor. Bu sayılar, 0 ve 1'lerden oluşan binary sayılardır. 
 N sayısının, "j" numaralı bitten, "i" numaralı bite kadar enjekte etmemiz isteniyor.
5.2

Binary to String: Given a real number between 0 and 1 (e.g., 0.72) that is passed in as a double, print the binary representation. If the number cannot be represented accurately in binary with at most 32 characters, print "ERROR:'

Hints:#743,#767,#773,#269,#297
 Herhangi bir reel sayı (Örn: 0.72) veriliyor. Bunun binary gösterimini (0 ve 1'lerden oluşan) yapınız. Eğer 32-bit ile ifade edilemiyors, "ERROR" yazdırın.

5.3
Flip Bit to Win: You have an integer and you can flip exactly one bit from a 0 to a 1. Write code to find the length of the longest sequence of 1s you could create.

EXAMPLE

Input: 1775 (or: 11011101111) Output: 8
 Hints: #759, #226, #374,#352 
 
 Herhangi bir tam sayının, binary hali veriliyor. Bu binary halde, herhangi bir 0 değerini 1 değerine dönüştürme şansınız var. Bunu yaparak elde edilebilecek en uzun 1 serisinin sayısını döndürün. Mesela 11011101111 sayısındaki ilk 0'ı 1'e dönüştürürsek 6 adet 1 art arda gelmiş olur. İkinci 0'ı 1'e dönüştürürsek 8 adet 1 art arda gelmiş olur. Dolayısı ile sonuç 8'dir.

5.4
Next Number: Given a positive integer, print the next smallest and the next largest number that have the same number of 1 bits in their binary representation.

Hints: #747, #7 75, #242,#372,#339,#358,#375,#390
Bir pozitif integer veriliyor. Bu integerin binary halindeki 1'lerle aynı sayıda 1 içeren, bir sonraki en küçük ve en büyük integer değerleri bulan bir fonksiyon yazın.

5.5
 Debugger: Explain what the following code does: ((n & (n-1)) == 0).

Hints:#757,#202,#267,#302,#346,#372,#383,#398
 
 Bu kodun ne yaptığını açıklayın: ((n & (n-1)) == 0)

5.6
Conversion: Write a function to determine the number of bits you would need to flip to convert integer A to integer B.

EXAMPLE

Input: 29 (or: 11101), 15 (or: 01111)

Output: 2

Hints: #336,#369

 İki tane integer veriliyor. örnek: 29 ve 15.  
 Bunların binary halleriyle (11101 ve 01111) düşünüldüğünde, A'yı B'ye çevirmek için değiştirilmesi gereken bit sayısını yazın. (11101 sayısını, 01111 sayısına çevirmek için 2 bit değiştirilmeli. ) 

5.7

  Pairwise Swap: Write a program to swap odd and even bits in an integer with as few instructions as possible (e.g., bit 0 and bit 1 are swapped, bit 2 and bit 3 are swapped, and so on).

Hints:#745,#248,#328,#355
 
 Çift sıradaki (örnek:0. bit, 2. bit, 4. bit)  bit ile, tek sıradaki bitleri (örnek: 1. bit, 3. bit, 5. bit) yer değiştirecek kodu yazın.

5.8

Draw Line: A monochrome screen is stored as a single array of bytes, allowing eight consecutive pixels to be stored in one byte. The screen has width w, where w is divisible by 8 (that is, no byte will be split across rows). The height of the screen, of course, can be derived from the length of the array and the width. Implement a function that draws a horizontal line from (xl, y) to ( x2, y).

The method signature should look something like:

drawline(byte[] screen, int width, int xl, int x2, int y) bu fonksiyon aracılığı ile yatay bir çizgi çizilmesi isteniyor.

Hints:#366,#387,#384,#397
Sıfırlardan oluşandan bir ekrana 1'lerden oluşan bir çizgi çizilecek.
 Çizginin hangi sütundan başlayacağını x1, hangi sütunda biteceğini x2, hangi satırda çizileceğini y1 ile göstereceğiz.

Örnek sonuç:
drawLine(screen, width, 1, 9, 1);

printScreen(screen, width);

00000000000000000000000000000000
01111111110000000000000000000000
00000000000000000000000000000000
00000000000000000000000000000000
@@@@@@@

6. Ünite soruları: Matematik ve Mantık sorular.
6.1 The Heavy Pill: You have 20 bottles of pills. 19 bottles have 1.0 gram pills, but one has pills of weight 1.1 grams. Given a scale that provides an exact measurement, how would you find the heavy bottle? You can only use the scale once. pg 122
20 adet ilaç şişesi var. 
19 ilaç şişesi 1.0 gramlık ilaçlardan, 1 ilaç şişesi ise 1.1 gramlık ilaçlardan bulunduruyor.
Tartıyı bir kez kullanmak şartı ile, hangi şişenin ağır olduğunu nasıl bulursun?

6.2 Basketball: You have a basketball hoop and someone says that you can play one of two games. Game 1: You get one shot to make the hoop. Game 2: You get three shots and you have to make two of three shots. If p is the probability of making a particular shot, for which values of p should you pick one game or the other? pg 123 

6.3 Dominos: There is an 8x8 chessboard in which two diagonally opposite corners have been cut off. You are given 31 dominos, and a single domino can cover exactly two squares. Can you use the 31 dominos to cover the entire board? Prove your answer (by providing an example or showing why it's impossible). pg 123 

6.4 Ants on a Triangle: There are three ants on different vertices of a triangle. What is the probability of collision (between any two or all of them) if they start walking on the sides of the triangle? Assume that each ant randomly picks a direction, with either direction being equally likely to be chosen, and that they walk at the same speed. Similarly, find the probability of collision with n ants on an n-vertex polygon. pg 123 

6.5 Jugs of Water: You have a five-quart jug, a three-quart jug, and an unlimited supply of water (but no measuring cups). How would you come up with exactly four quarts of water? Note that the jugs are oddly shaped, such that filling up exactly "half" of the jug would be impossible. pg 123 

6.6 Blue-Eyed Island: A bunch of people are living on an island, when a visitor comes with a strange order: all blue-eyed people must leave the island as soon as possible. There will be a flight out at 8:00pm every evening. Each person can see everyone else's eye color, but they do not know their own (nor is anyone allowed to tell them). Additionally, they do not know how many people have blue eyes, although they do know that at least one person does. How many days will it take the blue-eyed people to leave? pg113 

6.7 The Apocalypse: In the new post-apocalyptic world, the world queen is desperately concerned about the birth rate. Therefore, she decrees that all families should ensure that they have one girl or else they face massive fines. If all families abide by this policy-that is, they have continue to have children until they have one girl, at which point they immediately stop-what will the gender ratio of the new generation be? (Assume that the odds of someone having a boy or a girl on any given pregnancy is equal.) Solve this out logically and then write a computer simulation of it. pg 123 

6.8 The Egg Drop Problem: There is a building of 100 floors. If an egg drops from the Nth floor or above, it will break. If it's dropped from any floor below, it will not break. You're given two eggs. Find N, while minimizing the number of drops for the worst case. pg/24

6.9 100 Lockers: There are 100 closed lockers in a hallway. A man begins by opening all 100 lockers. Next, he closes every second locker. Then, on his third pass, he toggles every third locker (closes it if it is open or opens it if it is closed). This process continues for 100 passes, such that on each pass i, the man toggles every ith locker. After his 100th pass in the hallway, in which he toggles only locker #100, how many lockers are open? pg 124 
6. 10 Poison: You have 1000 bottles of soda, and exactly one is poisoned. You have 10 test strips which can be used to detect poison. A single drop of poison will turn the test strip positive permanently. You can put any number of drops on a test strip at once and you can reuse a test strip as many times as you'd like (as long as the results are negative). However, you can only run tests once per day and it takes seven days to return a result. How would you figure out the poisoned bottle in as few days as possible? Follow up: Write code to simulate your approach. pg 124 
 
 7. Ünite: Object-Oriented Programming: Nesneye yönelik programlama.

7.1 Deck of Cards: Design the data structures for a generic deck of cards. Explain how you would subclass the data structures to implement blackjack. pg127 

7.2 Call Center: Imagine you have a call center with three levels of employees: respondent, manager, and director. An incoming telephone call must be first allocated to a respondent who is free. If the respondent can't handle the call, he or she must escalate the call to a manager. If the manager is not free or not able to handle it, then the call should be escalated to a director. Design the classes and data structures for this problem. Implement a method dispatchCall () which assigns a call to the first available employee. pg127 

7.3 Jukebox: Design a musical jukebox using object-oriented principles. pg127

7.4 Parking Lot: Design a parking lot using object-oriented principles. pg 121

7.5 Online Book Reader: Design the data structures for an online book reader system.  pg127

7.6 Jigsaw: Implement an NxN jigsaw puzzle. Design the data structures and explain an algorithm to solve the puzzle. You can assume that you have a fitsWi th method which, when passed two puzzle edges, returns true if the two edges belong together. pg 128 

7 .7 Chat Server: Explain how you would design a chat server. In particular, provide details about the various backend components, classes, and methods. What would be the hardest problems to solve? pg 128 

7 .8 Othello: Othello is played as follows: Each Othello piece is white on one side and black on the other. When a piece is surrounded by its opponents on both the left and right sides, or both the top and bottom, it is said to be captured and its color is flipped. On your turn, you must capture at least one of your opponent's pieces. The game ends when either user has no more valid moves. The win is assigned to the person with the most pieces. Implement the object-oriented design for Othello. pg128 

7.9 Circular Array: Implement a CircularArray class that supports an array-like data structure which can be efficiently rotated. If possible, the class should use a generic type (also called a template), and should support iteration via the standard for (Obj o : circularArray) notation. pg 128 

7.10  Minesweeper: Design and implement a text-based Minesweeper game. Minesweeper is the classic single-player computer game where an NxN grid has B mines (or bombs) hidden across the grid. The remaining cells are either blank or have a number behind them. The numbers reflect the number of bombs in the surrounding eight cells. The user then uncovers a cell. If it is a bomb, the player loses. If it is a number, the number is exposed. If it is a blank cell, this cell and all adjacent blank cells (up to and including the surrounding numeric cells) are exposed. The player wins when all non-bomb cells are exposed. The player can also flag certain places as potential bombs. This doesn't affect game play, other than to block the user from accidentally clicking a cell that is thought to have a bomb. (Tip for the reader: if you're not familiar with this game, please play a few rounds on line first.) pg129

7.11 File System: Explain the data structures and algorithms that you would use to design an in-memory file system. Illustrate with an example in code where possible. pg 129 

7.12 Hash Table: Design and implement a hash table which uses chaining (linked lists) to handle collisions. pg 129 

@@@@@@@@@@@@
8. Ünite soruları: 
Solutions to Recursion and Dynamic Programming

8.1 Triple Step: A child is running up a staircase with n steps and can hop either 1 step, 2 steps, or 3 steps at a time. Implement a method to count how many possible ways the child can run up the stairs. pg134 
8.1:Bir çocuk, "n" basamaklı bir merdivene çıkar. Tek seferde 1 basamak, 2 basamak veya 3 basamak atlayabilir. Bu çocuğun kaç farklı yolla merdiveni çıkabileceğini gösteren bir yöntem yazın. (Rekürsif mantıkla düşünmüş. Çocuğun son adımının kaçlı olacağını düşünmüş. )

8.2 Robot in a Grid: Imagine a robot sitting on the upper left corner of grid with r rows and c columns. The robot can only move in two directions, right and down, but certain cells are "off limits" such that the robot cannot step on them. Design an algorithm to find a path for the robot from the top left to the bottom right. pg735 

8.2:Bir "grid" sol üst köşesinde, "r" satırı ve "c" sütununda bir robot olduğunu varsayın. Bu robot sadece sağa ve aşağıya hareket edebilir. Ancak robot, bazı hücrelere basamaz. Buna göre sağ alt köşeye gidebilecek yolu gösteren bir yöntem yazın.
-
8.3 Magic Index: A magic index in an array A[ 1 ... n-1] is defined to be an index such that A[i]= i. Given a sorted array of distinct integers, write a method to find a magic index, if one exists, in array A. FOLLOW UP What if the values are not distinct? pg 135 

8.3 Sihirli İndex: Bir Array var. Örnek: Dizi= 1, 4, 13,  3, 6, 7, 5, 11, 32, 9 
Burada: 3 ve 9 sihirli indexe sahiptir. Çünkü Dizi[3]= 3, Dizi[9]= 9 

8.4 Power Set: Write a method to return all subsets of a set. pg135
 8.4:  Bir kümenin tüm alt kümelerini döndürmek için bir yöntem yazın. pg135
 
8.5 Recursive Multiply: Write a recursive function to multiply two positive integers without using the * operator (or / operator). You can use addition, subtraction, and bit shifting, but you should minimize the number of those operations. pg 135 

8.5 "x" (Çarpı) işaretini kullanmadan iki pozitif tam sayıyı çarpmak için özyinelemeli bir fonksiyon yazın. Toplama, çıkarma ve bit kaydırma kullanabilirsiniz, ancak bu işlemlerin sayısını en aza indirmelisiniz.

8.6 Towers of Hanoi: In the classic problem of the Towers of Hanoi, you have 3 towers and N disks of different sizes which can slide onto any tower. The puzzle starts with disks sorted in ascending order of size from top to bottom (i.e., each disk sits on top of an even larger one). You have the following constraints: (1) Only one disk can be moved at a time. (2) A disk is slid off the top of one tower onto another tower. (3) A disk cannot be placed on top of a smaller disk. Write a program to move the disks from the first tower to the last using Stacks. pg 135

8.6  Klasik Hanoi Kulesi probleminde, 3 farklı kuleye ve herhangi bir kuleye kayabilecek, farklı boyutlarda N disklere sahipsiniz. Bulmaca, yukarıdan aşağıya doğru artan boyutta sıralanan disklerle başlar. Aşağıdaki kısıtlamalara sahipsiniz: (1) Bir seferde yalnızca bir disk taşınabilir. (2) Bir disk, bir kulenin tepesinden başka bir kulenin üzerine kaydırılır. (3) Bir disk, daha küçük bir diskin üzerine yerleştirilemez. Stacks kullanarak diskleri ilk kuleden sonuncuya taşımak için bir program yazın.

8.7 Permutations without duplications: Write a method to compute all permutations of a string of unique characters. pg 735 
 8.7   Benzersiz bir karakterlerden oluşan dizinin tüm permütasyonlarını hesaplamak için bir yöntem yazın. 

8.8 Permutations with Duplicates: Write a method to compute all permutations of a string whose characters are not necessarily unique. The list of permutations should not have duplicates. pg 735 
8.8  Karakterleri, "mutlaka benzersiz" demeyeceğimiz, yani benzersiz olma şartı olmayan bir dizenin tüm permütasyonlarını hesaplamak için bir yöntem yazın. Permütasyonların listesinde iki kopya bulunmamalıdır. 

8.9 Parens: Implement an algorithm to print all valid (i.e., properly opened and closed) combinations of n pairs of parentheses. EXAMPLE Input: 3 Output: (( () ) ) , ( () () ) , ( () ) () , () ( () ) , ()( ) () pg 136

8.9 n sayıdaki parantez çiftinin tüm geçerli kombinasyonlarını yazdırmak için bir algoritma uygulayın. (Yani doğru şekilde açılıp kapatılmış olanların.) ÖRNEK Giriş: 3 Çıkış: ((())), (() ()), (()) (), () (()), () () () pg 136

8.10 Paint Fill: Implement the"paint fill"function that one might see on many image editing programs. That is, given a screen (represented by a two-dimensional array of colors), a point, and a new color, fill in the surrounding area until the color changes from the original color. pg 136 
8.10  Resim düzenlemek için kullanılan birçok programda görebileceğiniz "boya dolgusu" işlevini uygulayın. Yani ekrana yeni bir renkte nokta konduğunda, (iki boyutlu renk dizisi ile temsil edilir) renk orijinal rengini kaybedene kadar etrafını doldurun.
8.11 Coins: Given an infinite number of quarters (25 cents), dimes (1O cents), nickels (5 cents), and pennies (1 cent), write code to calculate the number of ways of representing n cents. pg 136 

 8.11  Sınırsız sayıda 25 kuruş, 10 kuruş, 5 kuruş ve 1 kuruş verildiğinde, n kuruşa  tamamlama yollarını yazın. 
 
8.12 Eight Queens:Write an algorithm to print all ways of arranging eight queens on an 8x8 chess board so that none of them share the same row, column, or diagonal. In this case, "diagonal" means all diagonals, not just the two that bisect the board. pg 736 

 8.12  8x8 Satranç tahtasında, hiçbiri aynı sırayı, sütunu veya köşeyi paylaşmayacak şekilde sekiz kraliçeyi düzenlemenin tüm yollarını yazdırmak için bir algoritma yazın. (Sanırım kraliçe dediğinin ne olduğu önemli değil, herhangi bir taşı bu şekilde dizmek gerek. Mesela 1 rakamını sudokuda yerleştirmekle aynı mantık.)  Tahtanın yarısı değil, hepsi kullanılmalı. 
 
8.13 Stack of Boxes: You have a stack of n boxes, with widths w1, heights hi, and depths di. The boxes cannot be rotated and can only be stacked on top of one another if each box in the stack is strictly larger than the box above it in width, height, and depth. Implement a method to compute the height of the tallest possible stack. The height of a stack is the sum of the heights of each box. pg 136

8.13 Kutu stacki: "w1" genişliğine, "hi" yüksekliğine, "di" derinliğine sahip, n sayıda kutu yığınına sahipsiniz. Kutular döndürülemez ve yeni bir kutu koymak için, stackteki tüm kutuların, üstlerindeki her bir kutudan genişlik, yükseklik ve derinlik olarak kesinlikle büyük olması gerekir. Sadece bu şekilde üst üste istiflenebilir. (Sanırım piramit şeklinde dizilmesi gerektiğini söylüyor.) Mümkün olan en uzun stack yüksekliğini hesaplamak için bir yöntem uygulayın. Bir stack yüksekliği, her bir kutunun yüksekliğinin toplamıdır.
 
8.14 Boolean Evaluation: Given a boolean expression consisting of the symbols 0 (false), 1 (true), & (AND), | (OR), and ^(XOR), and a desired boolean result value result, implement a function to count the number of ways of parenthesizing the expression such that it evaluates to result.


8.14. Boolean değerlendirme (hesaplama): console.log(countEval('1^0|0|1', false)); // 2, correct
console.log(countEval('0&0&0&1^1|0', true)); // 30, should be 10!?!?!


@@@@@@@@@@@@@@@
Solutions to System Design and Scalability
9.1 Stock Data: Imagine you are building some sort of service that will be called by up to 1,000 client applications to get simple end-of-day stock price information (open, close, high, low). You may assume that you already have the data, and you can store it in any format you wish. How would you design the client-facing service that provides the information to client applications? You are responsible for the development, rollout, and ongoing monitoring and maintenance of the feed. Describe the different methods you considered and why you would recommend your approach. Your service can use any technologies you wish, and can distribute the information to the client applications in any mechanism you choose. pg 144 

9.1 Hisse Senedi Verileri: Gün sonu hisse senedi fiyat bilgilerini (açılış fiyatları, kapanış fiyatları, en yüksek fiyat, en düşük fiyat şeklinde) elde etmek için 1.000 kadar müşteri tarafından kullanılacak bir uygulama düşünün. Verilere zaten sahip olduğunuzu varsayabilir ve istediğiniz herhangi bir biçimde saklayabilirsiniz. Müşterilerin kullanacağı uygulamalara bilgi sağlayan hizmeti nasıl tasarlarsınız? Uygulamanın geliştirilmesinden, piyasaya sürülmesinden ve sürekli izlenmesinden ve bakımından siz sorumlusunuz. Düşündüğünüz farklı yöntemleri ve neden bu yaklaşımı önereceğinizi açıklayın. Servisiniz istediğiniz teknolojileri kullanabilir ve bilgileri diğer uygulamalarda müşterilere sunabilirsiniz. 

9.2 Social Network: How would you design the data structures for a very large social network like Facebook or Linkedln? Describe how you would design an algorithm to show the shortest path between two people (e.g., Me-> Bob-> Susan-> Jason-> You). pg 145 

 9.2 Sosyal Ağ: Facebook veya Linkedln gibi çok büyük sosyal ağlar için gereken veri yapılarını nasıl tasarlarsınız? İki kişi arasındaki en kısa yolu gösterecek bir algoritmayı nasıl tasarlayacağınızı açıklayın. (Örneğin: Me-> Bob-> Susan-> Jason-> Siz) 

9.3 Web Crawler: If you were designing a web crawler, how would you avoid getting into infinite loops? pg 745 
9.3 Web Crawler: Bir web crawler tasarlıyorsanız, sonsuz döngülere girmekten nasıl kaçınırsınız?

9.4 Duplicate URLs: You have 10 billion URLs. How do you detect the duplicate documents? In this case, assume "duplicate" means that the URLs are identical. pg 745 

9.5 Cache: Imagine a web server for a simplified search engine. This system has 100 machines to respond to search queries, which may then call out using processSearch(string query) to another cluster of machines to actually get the result. The machine which responds to a given query is chosen at random, so you cannot guarantee that the same machine will always respond to the same request. The method processSearch is very expensive. Design a caching mechanism to cache the results of the most recent queries. Be sure to explain how you would update the cache when data changes. pg 745 
9.5 Önbellek: Basitleştirilmiş bir arama motoru için bir web sunucusu hayal edin. Bu sistem, arama sorgularına cevap vermek için 100 makineye sahiptir, bu da sonucu elde etmek için processSearch (string query) komutunu başka bir makine kümesine kullanarak çağırabilir. Belirli bir sorguyu yanıtlayan makine rastgele seçilir, bu nedenle aynı makinenin her zaman aynı göreve cevap vereceğini garanti edemezsiniz. ProcessSearch yöntemi çok pahalıdır. En son sorguların sonuçlarını önbelleğe almak için bir önbellek mekanizması tasarlayın. Veri değiştiğinde önbelleği nasıl güncelleyeceğinizi açıkladığınızdan emin olun. 
9.6 Sales Rank: A large eCommerce company wishes to list the best-selling products, overall and by category. For example, one product might be the #1056th best-selling product overall but the #13th best-selling product under "Sports Equipment" and the #24th best-selling product under "Safety:· Describe how you would design this system. pg 745 

9.6 Satış Sıralaması: Büyük bir e-ticaret şirketi, tüm ürünlere  ve kategoriye göre en çok satan ürünleri listelemek istiyor. Örneğin, bir ürün genel olarak # 1056. sıradaki en çok satan ürün olabilir ama "Spor Malzemeleri" kategorisinde en çok satan 10. ürün olabilir.  "Güvenlik" :kategorisindeki 24. en çok satan ürün olabilir.
Bu sistemi nasıl tasarlayacağınızı açıklayın. 

9.7 Personal Financial Manager: Explain how you would design a personal financial manager (like Mint.com). This system would connect to your bank accounts, analyze your spending habits, and make recommendations. 

9.7 Kişisel Finans Yöneticisi: Mint.com gibi bir kişisel finans yöneticisini nasıl tasarlayacağınızı açıklayın. Bu sistem banka hesaplarınıza bağlanır, harcama alışkanlıklarınızı analiz eder ve önerilerde bulunur. 

9.8 Pastebin: Design a system like Pastebin, where a user can enter a piece of text and get a randomly generated URL for public access. pg745 
9.8 Pastebin: Bir kullanıcının bir metin girebileceği ve rastgele oluşturulmuş bir URL alabileceği Pastebin gibi bir sistem tasarlayın. 
@@@@@@@@@@

10. Ünite:
Solutions to Sorting and Searching

10.1 Sorted Merge: You are given two sorted arrays, A and B, where A has a large enough buffer at the end to hold B. Write a method to merge B into A in sorted order. pg149 
 10.1 Sıralanmış Birleştirme: A ve B olmak üzere iki sıralı dizi verilir; sıralı olarak  B'yi A'ya birleştirmek için bir yöntem yazın. (Birleştirince sıraları değişiyor.)

10.2 Group Anagrams: Write a method to sort an array of strings so that all the anagrams are next to each other. pg 150 
10.2 Grup Anagramları: Bir String dizisini sıralamak için öyle bir yöntem yazın ki tüm anagramlar yan yana olsun.
 Örnek: {"one", "neo", "kitap", "patik", "para", "arap"}

10.3 Search in Rotated Array: Given a sorted array of n integers that has been rotated an unknown number of times, write code to find an element in the array. You may assume that the array was originally sorted in increasing order. 
EXAMPLE 
input:find 5 in {15, 16, 19, 20, 25, 1, 3, 4, 5, 7, 10, 14} Output: 8 (the index of 5 in the array) pg 150

10.3 Döndürülmüş Dizi İçinde Ara: Bilinmeyen sayıda döndürülmüş sıralanmış bir n tam sayı dizisi verildiğinde, dizideki bir öğeyi bulmak için kod yazın. Dizinin başlangıçta artan düzende sıralandığını varsayabilirsiniz.   ÖRNEK : Dizideki 5'in indeksi Giriş: find 5 in {15, 16, 19, 20, 25, 1, 3, 4, 5, 7, 10, 14}  Çıktı: 8 
 Not: Binary search yapılacak, ama dizi "rotated" yani, ortasından sayısız kez döndürülmüş.

10.4 Sorted Search, No Size: You are given an array-like data structure Listy which lacks a size method. It does, however, have an elementAt ( i) method that returns the element at index i in 0( 1) time. If i is beyond the bounds of the data structure, it returns -1. (For this reason, the data structure only supports positive integers.) Given a Listy which contains sorted, positive integers, find the index at which an element x occurs. If x occurs multiple times, you may return any index. pg 150 
10.4 Sıralı Arama, size() Yok:  belli size() methodu olmayan, Listy adında, dizi-benzeri bir veri yapısı verilir.  Bununla birlikte, 0 indexindeki öğeyi O(1) zamanında döndüren bir elementAt(i) yöntemine sahiptir. Eğer veri yapısının sınırları dışındaysa, -1 döndürür. (Bu nedenle, veri yapısı sadece pozitif tamsayıları destekler.) Sıralı, pozitif tamsayılar içeren bir liste göz önüne alındığında, x öğesinin olduğu dizini bulun. X birden çok kez bulunursa, herhangi bir index döndürebilirsiniz. 
Not: elementAt(index) methodunu kullanarak, bunun tam tersini yapan yani herhangi elemanın indexini döndüren method yazmak.

10.5 Sparse Search: Given a sorted array of strings that is interspersed with empty strings, write a method to find the location of a given string.

 EXAMPLE 

Input: ball, {"at", "", "", "", "ball", "", "",  "car", "", "",  "dad", "", "" } 

Output: 4  

10.5 Seyrek Arama: Boşluklu bir dizi verildiğinde, verilen String yerini bulmak için bir yöntem yazın. 

10.6 Sort Big File: Imagine you have a 20 GB file with one string per line. Explain how you would sort the file. pg 150 
10.6 Büyük Dosyayı Sırala: Her bir satırında bir String (metin) olan 20 GB'lık bir dosya hayal edin. Dosyayı nasıl sıralayacağınızı açıklayın.

10.7 Missing Int: Given an input file with four billion non-negative integers, provide an algorithm to generate an integer that is not contained in the file. Assume you have 1 GB of memory available for this task. FOLLOW UP What if you have only 1O  MB of memory? Assume that all the values are distinct and we now have no more than one billion non-negative integers. pg750 

10.7 Kayıp tamsayı: Negatif olmayan dört milyar adet tamsayı içeren bir girdi dosyası verildiğinde, dosyada bulunmayan bir tamsayı üretmek için bir algoritma yazın (-sağlayın). Bu görev için 1 GB belleğinizin olduğunu varsayalım.  Takip Et: (Ek olarak soruyor sanırım.) Sadece 10 MB belleğiniz olsaydı ne yapardınız?  Tüm değerlerin farklı olduğunu ve şimdi bir milyardan fazla negatif olmayan tamsayıya sahip olmadığımızı varsayalım. 


10.8 Find Duplicates: You have an array with all the numbers from 1 to N, where N is at most 32,000. The array may have duplicate entries and you do not know what N is. With only 4 kilobytes of memory available, how would you print all duplicate elements in the array? pg 151 

10.8 Tekrarlanan Öğeleri Bul: N'nin değeri en büyük 32.000 olabilecek şekilde, 1'den N'ye kadar olan tüm sayıları içeren bir diziniz var. Dizinin yinelenen girişleri olabilir ve N'nin ne olduğunu bilmiyorsunuz. Yalnızca 4 kilobayt bellek alanınız varsa, dizideki tüm yinelenen öğeleri nasıl yazdırırsınız?

10.9 Sorted Matrix Search: Given an M x N matrix in which each row and each column is sorted in ascending order, write a method to find an element. pg 151 
10.9 Sıralı Matris Arama: Her satırın ve her sütunun artan bir şekilde sıralandığı, düzenli bir M x N matrisinin içindeki herhangi bir elemanı bulmak için bir yöntem yazın. 

10.10 Rank from Stream: Imagine you are reading in a stream of integers. Periodically, you wish to be able to look up the rank of a number x (the number of values less than or equal to x). Implement the data structures and algorithms to support these operations. That is, implement the method track(int x), which is called when each number is generated, and the method getRankOfNumber(int x), which returns the number of values less than or equal to x (not including x itself).  pg151
EXAMPLE 
Stream(inorderofappearance):5, 1, 4, 4, 5, 9, 7, 13, 3 
getRankOfNumber(1) = 0 
getRankOfNumber(3) = 1 
getRankOfNumber(4) = 3  

(Not: Bir Stream x elemanından küçük veya ona eşit (kendisi hariç) kaç eleman olduğunu gösteren method yazınız)

10.10 Stream'den derece (rank) bulmak: Bir tam sayı akışını (Burada "in" var, o yüzden "akışında" olabilir ama mantıklı gelmedi.) okuduğunuzu hayal edin. Periyodik olarak, x sayısının sırasına bakmak istiyorsunuz. (x'den küçük veya ona eşit olan değerlerin sayısı.)  (Bundan sonrasını pek anlayamadım.) Bu işlemleri desteklemek için veri yapılarını ve algoritmaları uygulayın. Diğer bir deyişle, her sayı üretildiğinde çağrılan yöntem izini (int x) ve x'e eşit veya daha küçük (x değerini içermeyen) değerlerini döndüren getRankOfNumber (int x) yöntemini uygulayın.  Örnek:   Stream(inorderofappearance):5, 1, 4, 4, 5, 9, 7, 13, 3 
getRankOfNumber(1) = 0 
getRankOfNumber(3) = 1 
getRankOfNumber(4) = 3  

10.11 Peaks and Valleys: In an array of integers, a "peak" is an element which is greater than or equal to the adjacent integers and a "valley" is an element which is less than or equal to the adjacent integers. For example, in the array
{5, 8, 6, 2, 3, 4, 6}, {8, 6} are peaks and {5, 2} are valleys. Given an array of integers, sort the array into an alternating sequence of peaks and valleys. pg 151 
EXAMPLE
 Input: {5, 3, 1, 2, 3} 
Output: {5, 1, 3, 2, 3} 

  10.11 Tepeler ve Vadiler: Bir tamsayı dizisinde,   Tepe: Bitişik tamsayılara eşit veya ondan daha büyük bir elementtir. Vadi: Bitişik tamsayılara eşit veya ondan daha küçük bir elementtir.  Örneğin, {5, 8, 6, 2, 3, 4, 6} dizisinde,  {8, 6} tepe noktaları   {5, 2} vadiler Bir tamsayı dizisi verildiğinde, bu diziyi değişen bir tepe ve vadiler dizisine göre sıralayın.  
 (Bir tepe, bir vadi, bir tepe, bir vadi olacak şekilde sıralama)
@@@@@@@@@@
11. Ünite: Test

11.1 Mistake: Find the mistake(s) in the following code:
unsigned int i; 
for (i = 100; i >= 0; --i)
printf("%d\n", i); 

11.1  Hata: Takip eden kodların içinde hataları bulun :
unsigned int i; 
for (i = 100; i >= 0; --i)
printf("%d\n", i); 

11.2 Random Crashes: You are given the source to an application which crashes when it is run. After
running it ten times in a debugger, you find it never crashes in the same place. The application is
single threaded, and uses only the C standard library. What programming errors could be causing
this crash? How would you test each one? pg 157
11.2 Rastgele Çökmeler: Bir uygulama çalıştırıldığın çöküyor. On kez debug yaptığınızda, aynı yerde asla çökmediğini fark ediyorsunuz. Uygulama yalnızca standart C kütüphanesini kullanıyor. Bu çökmeler hangi programlama hatalarından kaynaklanabilir?
 Her birini nasıl test edersiniz? 

11.3 Chess Test: We have the following method used in a chess game: boolean canMoveTo(int x,
int y). This method is part of the Piece class and returns whether or not the piece can move to
position (x, y). Explain how you would test this method.
pg157 

11.3 Satranç Testi: Bir satranç oyununda kullanılan aşağıdaki gibi bir yöntemimiz var: 
boolean canMoveTo (int x, int y).   Bu yöntem, Piece sınıfının bir parçasıdır ve position(x, y) ile parçanın hareket edip edemeyeceğini  döndürür. Bu yöntemi nasıl test edeceğinizi açıklayın.

11.4 No Test Tools: How would you "load test" a webpage without using any test tools? 

11.4 Test Aracı Yok: Bir web sayfası için "yükleme testini" test aracı olmadan nasıl yaparsınız?

11.5 Test a Pen: How would you test a pen? 

11.5 Kalemi Test Et: Kalemi nasıl test edersiniz?

11.6 Test an ATM: How would you test an ATM in a distributed banking system? 

11.6 ATM'yi Test Etme: Dağıtık bankacılık sistemindeki bir ATM'yi nasıl test edersiniz? 
 
12. Ünite: C and C++
12.1 Last K Lines: Write a method to print the last Klines of an input file using C ++. pg163
12.1 Son K Satırı: C ++ kullanarak bir girdi dosyasının son K (tane) satırını yazdırmak için bir yöntem yazın.  

12.2 Reverse String: Implement a function void reverse(char* str) in C or C++ which reverses a nullterminated string. 

12.2  String'i tersine çevirme: C veya C ++ 'da  null-terminated stringi tersine çeviren "reverse(char * str)" void işlevini uygular. 

12.3 Hash Table vs STL Map: Compare and contrast a hash table and an STL map. How is a hash table implemented? If the number of inputs is small, which data structure options can be used instead of a hash table? 
12.3 Hash Table vs STL Map: Hash Table vs STL Map haritasını karşılaştırın. Bir Hash Table nasıl uygulanır? 
Girdi sayısı az ise,  Hash Table yerine hangi veri yapısı seçenekleri kullanılabilir? 

12.4 Virtual Functions: How do virtual functions work in C++? 
12.4 Sanal İşlevler: Sanal işlevler C ++ 'da nasıl çalışır?

12.5 Shallow vs Deep Copy: What is the difference between deep copy and shallow copy? Explain how
you would use each. 
12.5  Sığ ve Derin Kopyalama: Derin kopya ile sığ kopya arasındaki fark nedir? Her birini nasıl kullacağını açıkla.

12.6 Volatile: What is the significance of the keyword "volatile" in C? 
12.6  Uçucu(Volatile): C'deki "uçucu" ("Volatile") anahtar kelimenin anlamı nedir?

12.7 Virtual Base Class: Why does a destructor in base class need to be declared virtual? 

12.7  Sanal Temel Sınıf: Temel sınıftaki bir 'destructor-yıkıcı' methodun sanal olarak tanımlanmasının sebebi nedir?

12.8 Copy Node: Write a method that takes a pointer to a Node structure as a parameter and returns a
complete copy of the passed in data structure. The Node data structure contains two pointers to
other Nodes. 

12.8 Node'u kopyala: Bir Node için pointer'ı parametre olarak alan ve bunu kopyalayan bir method yazın.
Bu Node veriyapısı, diğer Node'lara dair iki pointer içermektedir.

12.9 Smart Pointer: Write a smart pointer class. A smart pointer is a data type, usually implemented
with templates, that simulates a pointer while also providing automatic garbage collection. It
automatically counts the number of references to a SmartPointer<T*> object and frees the
object of type T when the reference count hits zero. 

12.9  Akıllı İşaretçi: Bir akıllı işaretçi sınıfı yazın. Akıllı işaretçi, otomatik çöp toplama sağlarken aynı zamanda bir işaretçiyi simüle eden şablonlarla uygulanabilen bir veri türüdür.    Bir SmartPointer <T *> nesnesine yapılan referansları otomatik olarak sayar ve referans sayısı sıfıra ulaştığında T tipi nesneyi serbest bırakır.  

12.10 Malloc: Write an aligned malloc and free function that supports allocating memory such that the
memory address returned is divisible by a specific power of two.
EXAMPLE
align_malloc (1000, 128) will return a memory address that is a multiple of 128 and that points
to memory of size 1000 bytes.
aligned_free() will free memory allocated by align_malloc. 
12.10  Malloc: (Bu soruyu da anlamadım. Anca bu kadar oldu.) Öyle bir hizalanmış malloc yazın ki, hafıza tahsis edilmesini desteklesin. Dönen hafıza adresi, ikisinin belirli bir gücü ile bölünebilir.
ÖRNEK
align_malloc (1000, 128), 128 olan ve bu noktaların katı olan bir hafıza adresini döndürür.
1000 bayt boyutunda
align_free () align_malloc tarafından ayrılan belleği boşaltır.


12.11 20 Alloc: Write a function in C called my2DA1loc which allocates a two-dimensional array.
Minimize the number of calls to malloc and make sure that the memory is accessible by the
notation arr [ i] [ j]. 

12.11  20 Alloc: C'ye iki boyutlu bir array tahsis eden my2DA1loc adlı bir fonksiyon yazın. Malloc'a yapılan çağrı sayısını en aza indirin ve hafızaya [i] [j] notasyonu ile erişilebildiğinden emin olun.  
@@@@@@@@@

13 Ünite: Java
13.1 Private Constructor: In terms of inheritance, what is the effect of keeping a constructor private? 
13.1 Private Constructor: Kalıtım yönünden bakıldığında, bir constructor methodu private yapmanın etkisi nedir?

13.2 Return from Finally: In Java, does the finally block get executed if we insert a return statement
inside the try block of a try-catch-finally? 
13.2 Return from Finally: Java'da, bir try-catch-finally içinde, try bloğu içine return yazılırsa kod çalışır mı?

13.3 Final, etc.: What is the difference between final, finally, and "deneme try"? 

https://www.geeksforgeeks.org/g-fact-24-finalfinally-and-finalize-in-java/

13.4 Generics vs. Templates: Explain the difference between templates in C ++ and generics in Java. 
13.4: JAvadaki generics ile C'deki Templates farkı.

13.5 TreeMap, HashMap, LinkedHashMap: Explain the differences between TreeMap, HashMap, and
LinkedHashMap. Provide an example of when each one would be best. 

13.5 TreeMap, HashMap, LinkedHashMap: bu veri yapıları arasındaki fark.

13.6 Object Reflection: Explain what object reflection is in Java and why it is useful. 

13.6 Object Reflection: Reflection ile ne yapıldığını açıklayın.

13.7 Lambda Expressions: There is a class Country that has methods getContinent() and
getPopulation(). Write a function int getPopulation(List<Country> countries,
String continent) that computes the total population of a given continent, given a list of all
countries and the name of a continent. 

13.7:  Lambda Expressions: Country diye bir sınıf var. getContinent() ve getPopulation() diye iki methodu var. 
 getPopulation(List<Country> countries,
String continent) tüm ülkelerin ve kıtanın ismi verildiğinde, toplam nüfusu veren bir method yazın.
 
13.8 Lambda Random: Using Lambda expressions, write a function List<Integer>
getRandomSubset ( List< Integer> list) that returns a random subset of arbitrary size. All
subsets (including the empty set) should be equally likely to be chosen. 

13.8: Bu listeyi parametre olarak alan bir getRandomSubset ( List< Integer> list) methodu yazın.
Listenin alt kümelerinden herhangi birisini rastgele olarak döndürsün.
 

14. Ünite: Database
14.1 Multiple Apartments: Write a SQL query to get a list of tenants who are renting more than one
apartment. 
14.1 Birden çok ev: Birden fazla evi kiralayan kiracıların listesisni getirmek için bir SQL sorgusu yazın.

14.2 Open Requests: Write a SQL query to get a list of all buildings and the number of open requests
(Requests in which status equals 'Open'). 
SELECT r.*, b.buildingName FROM ctci.Requests as r 
		   JOIN ctci.Apartments as a ON r.apartmentID= a.apartmentID
		   JOIN ctci.Buildings as b ON a.buildingID= b.buildingID
           where r.status="Open";
                            
14.2 Açık Talepler:  Tüm binaların bir listesini ve açık taleplerin numarasını almak için bir SQL sorgusu yazın
('Açık' anlamına gelen talepler.)

14.3 Close All Requests: Building #11 is undergoing a major renovation. Implement a query to close all
requests from apartments in this building. 
UPDATE ctci.Requests r
JOIN ctci.Apartments as a ON r.apartmentID= a.apartmentID
		   JOIN ctci.Buildings as b ON a.buildingID= b.buildingID
           SET r.status ="Close"
		   where r.status="Open"
                            
	    	
14.3 Tüm Talepleri Kapatın:  11. bina, büyük bir tadilattan geçiyor. Bu binadaki dairelerin taleplerinin hepsini kapatmak için bir sorgu uygulayın.

14.4 Joins: What are the different types of joins? Please explain how they differ and why certain types
are better in certain situations. 
(https://www.w3schools.com/sql/sql_join.asp) 
14.4 (Joins):  Farklı Joins tipleri nelerdir? Lütfen nasıl farklı olduklarını ve belirli tiplerin bazı durumlarda neden daha iyi olduğunu açıklayın.

14.5 Denormalization: What is denormalization? Explain the pros and cons. 
14.5 Denormalizasyon: Denormalizasyon nedir? Artılarını ve eksilerini açıklar.

14.6 Entity-Relationship Diagram: Draw an entity-relationship diagram for a database with companies,
people, and professionals (people who work for companies). 
14.6 Şirketler, insânlar ve uzmanlar arasında ilişki diagramlarını oluşturun.


14.7 Design Grade Database: Imagine a simple database storing information for students' grades.
Design what this database might look like and provide a SQL query to return a list of the honor roll
students (top 10%), sorted by their grade point average. 

14.7 Mezuniyet Veritabanı:  Öğrencilerin notları için bilgi depolayan basit bir veritabanı düşünün.  Bu veritabanının neye benzeyeceğini tasarlayın ve öğrencilerin (%10) not ortalamasına göre sıralandıkları bir şeref listesi oluşturmak için SQL sorgusu yapın. 

15: Threadler ve Locklar

15.1 Thread vs. Process: What's the difference between a thread and a process? 
15.1  İş parçacığına karşı işlem(Süreç):  İş parçacığı ile bir işlem arasındaki fark nedir?

15.2 Context Switch: How would you measure the time spent in a context switch? 
  15.2 Context Switch (Şalter Bağlantısı):  Context Switch'te harcanan zamanı nasıl ölçersiniz?
15.3 Dining Philosophers: In the famous dining philosophers problem, a bunch of philosophers are
sitting around a circular table with one chopstick between each of them. A philosopher needs both
chopsticks to eat, and always picks up the left chopstick before the right one. A deadlock could
potentially occur if all the philosophers reached for the left chopstick atthe same time. Using threads
and locks, implement a simulation of the dining philosophers problem that prevents deadlocks. 
  15.3 Yemek Filozofları:  Ünlü yemek filozofları probleminde, bir grup filozof dairesel bir masanın etrafında oturuyor ve her filozof arasında bir yemek çubuğu bulunuyor.  Bir filozofun yemek yiyebilmesi için iki çubuğa ihtiyacı var ve her zaman sağdaki çubuktan önce soldaki çubuğu alır. Tüm filozoflar aynı anda önce soldaki çubuğu alırsa kilitlenme yaşanır.  (Çünkü iki çubuğa ihtiyaçları vardır ama hepsi soldakini alırsa, sağlarında çubuk kalmaz ve hiçbiri yemek yiyemez.) İşlem parçacığı kullanarak, bu problemin kilitlenmesini önleyen bir simülasyon uygulayın. 
15.4 Deadlock-Free Class: Design a class which provides a lock only if there are no possible deadlocks. 
 15.4 Deadlock-Free Sınıfı: Kilitlenme olmadığında, kilitlenmeyi sağlayan bir sınıf tasarlayın.
15.5 Call In Order: Suppose we have the following code:
public class Foo {
public Foo() { ... }
public void first() { ... }
public void second() { ... }
public void third() { ... }
}
The same instance of Foo will be passed to three different threads. ThreadA will call first threadB
will call second, and thread( will call third. Design a mechanism to ensure that first is called
before second and second is called before third. 
  15.5 Sırayla Ara:  Aşağıdaki gibi bir kodumuz olduğunu varsayalım:  public class Foo {
public Foo() { ... }
public void first() { ... }
public void second() { ... }
public void third() { ... }
}
Aynı 'Foo' üç farklı iş parçacığına iletilecek. ThreadA ilk ThreadB'yi arayacak sonra
ikinciyi arayacak ve son olarak üçüncüyü arayacak.  Arama sırasını tersine alacak bir mekanizma tasarlayın.
15.6 Synchronized Methods: You are given a class with synchronized method A and a normal
method B. If you have two threads in one instance of a program, can they both execute A at the
same time? Can they execute A and B at the same time?
  15.6  Senkronize Metotlar:  Senkronize metot A sınıfınız ve normal metot B sınıfınız var.  Eğer programın iki iş parçacıklı bir örneği varsa, ikisini de A sınıfı ile yapabilir misiniz? Veya A ve B sınıfını aynı anda kullanabilir misiniz? 

15.7 FizzBuzz: In the classic problem FizzBuzz, you are told to print the numbers from 1 to n. However,
when the number is divisible by 3, print "Fizz''. When it is divisible by 5, print "Buzz''. When it is
divisible by 3 and 5, print"FizzBuzz''. In this problem, you are asked to do this in a multithreaded way.
Implement a multithreaded version of FizzBuzz with four threads. One thread checks for divisibility
of 3 and prints"Fizz''. Another thread is responsible for divisibility of 5 and prints"Buzz''. A third thread
is responsible for divisibility of 3 and 5 and prints "FizzBuzz''. A fourth thread does the numbers. ,
   15.7
FizzBuzz:  Klasik FizzBuzz probleminde, 1'den n'ye kadar olan sayıları yazdırmanız isteniyor.
Sayı 3 ile bölünebiliyorsa: "Fizz"  Sayı 5 ile bölünebiliyorsa: "Buzz" Hem 3'e hem de 5'e bölünebiliyorsa:  "FizzBuzz '' yazdırılabilir. Bu problemi,  çok iş parçacıklı bir şekilde (multithreaded) ile yapmanız isteniyor. Dört iş parçacığı ile çok iş parçacıklı bir FizzBuzz sürümü uygulayın. Bir treaded 3 ile bölünebilirliği kontrol eder ve "Fizz '" yazar. Başka bir treaded 5 ile bölünebilirliği kontrol eder ve "Buzz" yazarr.  Üçüncü treaded ise hem 3 ile hem de 5 ile bölünebilirliğini kontrol eder ve "FizzBuzz '" yazar. 
@@@@@@@@@@@
16: Ek-Sorular: Orta Derece
16.1 Number Swapper: Write a function to swap a number in place (that is, without temporary variables). 

16.2 Word Frequencies: Design a method to find the frequency of occurrences of any given word in a
book. What if we were running this algorithm multiple times? 

16.3 Intersection: Given two straight line segments (represented as a start point and an end point),
compute the point of intersection, if any. 

16.4 Tic Tac Win: Design an algorithm to figure out if someone has won a game of tic-tac-toe

16.5 Factorial zeros: Write an algorithm which computes the number of trailing zeros in n factorial. 

16.6 Smallest Difference: Given two arrays of integers, compute the pair of values (one value in each
array) with the smallest (non-negative) difference. Return the difference.
EXAMPLE
Input: {l, 3, 15, 11, 2}, {23, 127, 235, 19, 8}
Output: 3. That is, the pair (11, 8). 

16.7 Number Max: Write a method that finds the maximum of two numbers. You should not use if else
or any other comparison operator. 

16.8 English Int: Given any integer, print an English phrase that describes the integer (e.g., "One
Thousand, Two Hundred Thirty Four"). 

16.9 Operations: Write methods to implement the multiply, subtract, and divide operations for integers.
The results of all of these are integers. Use only the add operator. 

16.10 Living People: Given a list of people with their birth and death years, implement a method to
compute the year with the most number of people alive. You may assume that all people were born
between 1900 and 2000 (inclusive). If a person was alive during any portion of that year, they should
be included in that year's count. For example, Person (birth= 1908, death= 1909) is included in the
counts for both 1908 and 1909. 

16.11 Diving Board: You are building a diving board by placing a bunch of planks of wood end-to-end.
There are two types of planks, one of length shorter and one of length longer. You must use
exactly K planks of wood. Write a method to generate all possible lengths for the diving board

16.12 XML Encoding: Since XML is very verbose, you are given a way of encoding it where each tag gets
mapped to a pre-defined integer value. The language/grammar is as follows:
Element --> Tag Attributes END Children END
Attribute --> Tag Value
END --> 0
Tag --> some predefined mapping to int
Value --> string value
For example, the following XML might be converted into the compressed string below (assuming a
mapping of family -> 1, person ->2, firstName -> 3, lastName -> 4, state
-> 5).
<family lastName="McDowell" state="CA">
<person firstName="Gayle">Some Message</person>
</family>
Becomes:
1 4 McDowell 5 CA 0 2 3 Gayle 0 Some Message 0 0
Write code to print the encoded version of an XML element (passed in Element and Attribute
objects). 

16.13 Bisect Squares: Given two squares on a two-dimensional plane, find a line that would cut these two
squares in half. Assume that the top and the bottom sides of the square run parallel to the x-axis. 

16.14 Best Line: Given a two-dimensional graph with points on it, find a line which passes the most
number of points. 

16.15 Master Mind: The G ame of Master Mind is played as follows:
The computer has four slots, and each slot will contain a ball that is red (R), yellow (Y), green (G) or
blue (B). For example, the computer might have RGGB (Slot #1 is red, Slots #2 and #3 are green, Slot
#4 is blue).
You, the user, are trying to guess the solution. You might, for example, guess YRGB.
When you guess the correct color for the correct slot, you get a "hit:' If you guess a color that exists
but is in the wrong slot, you get a "pseudo-hit:' Note that a slot that is a hit can never count as a
pseudo-hit.
For example, if the actual solution is RGBY and you guess GGRR, you have one hit and one pseudohit
Write a method that, given a guess and a solution, returns the number of hits and pseudo-hits.
pg 183 

16.16 Sub Sort: Given an array of integers, write a method to find indices m and n such that if you sorted
elements m through n, the entire array would be sorted. Minimize n - m (that is, find the smallest
such sequence).
EXAMPLE
Input: 1, 2, 4, 7, 10, 11, 7, 12, 6, 7, 16, 18, 19
Output: (3, 9) 

16.17 Contiguous Sequence: You are given an array of integers (both positive and negative). Find the
contiguous sequence with the largest sum. Return the sum.
EXAMPLE
Input: 2, -8, 3, -2, 4, -10
Output: 5 ( i. e • , { 3, -2, 4} ) 

16.18 Pattern Matching: You are given two strings, pattern and value. The pattern string consists of
just the letters a and b, describing a pattern within a string. For example, the string catcatgocatgo
matches the pattern aabab (where cat is a and go is b). It also matches patterns like a, ab, and b.
Write a method to determine if value matches pattern. 

16.19 Pond Sizes: You have an integer matrix representing a plot of land, where the value at that location
represents the height above sea level. A value of zero indicates water. A pond is a region of water
connected vertically, horizontally, or diagonally. The size of the pond is the total number of
connected water cells. Write a method to compute the sizes of all ponds in the matrix.
EXAMPLE
Input:
0 2 1 0
0 1 0 1
1 1 0 1
0 1 0 1
Output: 2, 4, 1 (in any order) 

16.20 T9: On old cell phones, users typed on a numeric keypad and the phone would provide a list of words
that matched these numbers. Each digit mapped to a set of O - 4 letters. Implement an algorithm
to return a list of matching words, given a sequence of digits. You are provided a list of valid words
(provided in whatever data structure you'd like). The mapping is shown in the diagram below:
EXAMPLE
Input: 8733
Output: tree, used 

16.21 Sum Swap: Given two arrays of integers, find a pair of values (one value from each array) that you
can swap to give the two arrays the same sum.
EXAMPLE
lnput:{4, 1, 2, 1, 1, 2}and{3, 6, 3, 3}
Output: {1, 3} 

16.22 Langton's Ant: An ant is sitting on an infinite grid of white and black squares. It initially faces right.
At each step, it does the following:
(1) At a white square, flip the color of the square, turn 90 degrees right (clockwise), and move forward
one unit.
(2) At a black square, flip the color of the square, turn 90 degrees left (counter-clockwise), and move
forward one unit.
Write a program to simulate the first K moves that the ant makes and print the final board as a grid.
Note that you are not provided with the data structure to represent the grid. This is something you
must design yourself. The only input to your method is K. You should print the final grid and return
nothing. The method signature might be something like void printKMoves ( int K). 

16.23 Rand7 from Rand 5: Implement a method rand7 () given rand S (). That is, given a method that
generates a random number between O and 4 (inclusive), write a method that generates a random
number between O and 6 (inclusive). 

16.24 Pairs with Sum: Design an algorithm to find all pairs of integers within an array which sum to a
specified value. 

16.25 LRU Cache: Design and build a "least recently used" cache, which evicts the least recently used item.
The cache should map from keys to values (allowing you to insert and retrieve a value associated
with a particular key) and be initialized with a max size. When it is full, it should evict the least
recently used item. You can assume the keys are integers and the values are strings

16.26 Calculator: Given an arithmetic equation consisting of positive integers,+,-,* and/ (no parentheses),
compute the result.
EXAMPLE
Input: 2*3+5/6*3+15 
Output: 23.5 

@@@@@@@@@@@@@@@@@
16: Ek-Sorular: Zor  
17 .1 Add Without Plus: Write a function that adds two numbers. You should not use+ or any arithmetic
operators. 

17 .2 Shuffle: Write a method to shuffle a deck of cards. It must be a perfect shuffle-in other words, each
of the 52! permutations of the deck has to be equally likely. Assume that you are given a random
number generator which is perfect. 

17 .3 Random Set: Write a method to randomly generate a set of m integers from an array of size n. Each
element must have equal probability of being chosen.

17 .4 Missing Number: An array A contains all the integers from O to n, except for one number which
is missing. In this problem, we cannot access an entire integer in A with a single operation. The
elements of A are represented in binary, and the only operation we can use to access them is "fetch
the jth bit of A[i];' which takes constant time. Write code to find the missing integer. Can you do it
in O(n) time? 

17.5 Letters and Numbers: Given an array filled with letters and numbers, find the longest subarray with
an equal number of letters and numbers. 

17 .6 Count of 2s: Write a method to count the number of 2s between O and n. 

17.7 Baby Names: Each year, the government releases a list of the 10,000 most common baby names
and their frequencies (the number of babies with that name). The only problem with this is that
some names have multiple spellings. For example, "John" and ''.Jon" are essentially the same name
but would be listed separately in the list. Given two lists, one of names/frequencies and the other
of pairs of equivalent names, write an algorithm to print a new list of the true frequency of each
name. Note that if John and Jon are synonyms, and Jon and Johnny are synonyms, then John and
Johnny are synonyms. (It is both transitive and symmetric.) In the final list, any name can be used
as the "real" name.
EXAMPLE
Input:
Names: John (15), Jon (12), Chris (13), Kris (4), Christopher (19)
Synonyms: (Jon, John), (John, Johnny), (Chris, Kris), (Chris, Christopher)
Output: John (27), Kris (36) 

17.8 Circus Tower: A circus is designing a tower routine consisting of people standing atop one another's
shoulders. For practical and aesthetic reasons, each person must be both shorter and lighter than
the person below him or her. Given the heights and weights of each person in the circus, write a
method to compute the largest possible number of people in such a tower. 

17 .9 Kth Multiple: Design an algorithm to find the kth number such that the only prime factors are 3, 5,
and 7. Note that 3, 5, and 7 do not have to be factors, but it should not have any other prime factors.
For example, the first several multiples would be (in order) 1, 3, 5, 7, 9, 15, 21. 

17 .10 Majority Element: A majority element is an element that makes up more than half of the items in
an array. Given a positive integers array, find the majority element. If there is no majority element,
return -1. Do this in O(N) time and 0(1) space.
Input: 1 2 5 9 5 9 5 5 5
Output: 5 


17 .11 Word Distance: You have a large text file containing words. Given any two words, find the shortest
distance (in terms of number of words) between them in the file. If the operation will be repeated
many times for the same file (but different pairs of words), can you optimize your solution? 


17.12 BiNode: Consider a simple data structure called BiNode, which has pointers to two other nodes. The
data structure BiNode could be used to represent both a binary tree (where node1 is the left node
and node2 is the right node) or a doubly linked list (where node1 is the previous node and node2
is the next node). Implement a method to convert a binary search tree (implemented with BiNode)
into a doubly linked list. The values should be kept in order and the operation should be performed
in place (that is, on the original data structure). 


17.13 Re-Space: Oh, no! You have accidentally removed all spaces, punctuation, and capitalization in a
lengthy document. A sentence like "I reset the c omputer. It still didn't boot!"
became "iresetthecomputeri tstilldidntboot''. You'll deal with the punctuation and capitalization later; right now you need to re-insert the spaces. Most of the words are in a dictionary but
a few are not. Given a dictionary (a list of strings) and the document (a string), design an algorithm
to unconcatenate the document in a way that minimizes the number of unrecognized characters.
EXAMPLE
Input jesslookedjustliketimherbrother
Output: jess looked just like tim her brother (7 unrecognized characters)
17 .14 Smallest K: Design an algorithm to find the smallest K numbers in an array

17.15 Longest Word: Given a list of words, write a program to find the longest word made of other words
in the list.' 

17.16 The Masseuse: A popular masseuse receives a sequence of back-to-back appointment requests
and is debating which ones to accept. She needs a 15-minute break between appointments and
therefore she cannot accept any adjacent requests. Given a sequence of back-to-back appointment requests (all multiples of 15 minutes, none overlap, and none can be moved), find the optimal
(highest total booked minutes) set the masseuse can honor. Return the number of minutes.
EXAMPLE
Input: {30, 15, 60, 75, 45, 15, 15, 45}
Output180 minutes ({30, 60, 45, 45}). 

17.17 Multi Search: Given a string band an array of smaller strings T, design a method to search b for
each small string in T. 

17 .18 Shortest Supersequence: You are given two arrays, one shorter (with all distinct elements) and one
longer. Find the shortest subarray in the longer array that contains all the elements in the shorter
array. The items can appear in any order.
EXAMPLE
Input:
{1, 5, 9}
{7, 5, 9, 0, 2, 1, 3, 5. 7, 9. 1, 1, 5, 8, 8, 9, 7}
Output:[7, 10] (the underlined portion above) 

17.19 Missing Two: You are given an array with all the numbers from 1 to N appearing exactly once,
except for one number that is missing. How can you find the missing number in O(N) time and
0( 1) space? What if there were two numbers missing? 

17.20 Continuous Median: Numbers are randomly generated and passed to a method. Write a program
to find and maintain the median value as new values are generated. 

17.21 Volume of Histogram: Imagine a histogram (bar graph). Design an algorithm to compute the
volume of water it could hold if someone poured water across the top. You can assume that each
histogram bar has width 1.
EXAMPLE
lnput{0, 0, 4, 0, 0, 6, 0, 0, 3, 0, 5, 0, 1, 0, 0, 0}
(Black bars are the histogram. Gray is water.) 

Output:26 

17.22 Word Transformer: Given two words of equal length that are in a dictionary, write a method to
transform one word into another word by changing only one letter at a time. The new word you get
in each step must be in the dictionary.
EXAMPLE
Input: DAMP, LIKE
Output: DAMP-> LAMP-> LIMP-> LIME-> LIKE 

17.23 Max Square Matrix: Imagine you have a square matrix, where each cell (pixel) is either black or
white. Design an algorithm to find the maximum subsquare such that all four borders are filled with
black pixels

17.24 Max Submatrix: Given an NxN matrix of positive and negative integers, write code to find the
submatrix with the largest possible sum.

17 .25 Word Rectangle: Given a list of millions of words, design an algorithm to create the largest possible
rectangle of letters such that every row forms a word (reading left to right) and every column forms
a word (reading top to bottom). The words need not be chosen consecutively from the list, but all
rows must be the same length and all columns must be the same height. 

17.26 Sparse Similarity: The similarity of two documents (each with distinct words) is defined to be the
size of the intersection divided by the size of the union. For example, if the documents consist of
integers, the similarity of {1, 5, 3} and { 1, 7, 2, 3} is 0. 4, because the intersection has size
2 and the union has size 5.
We have a long list of documents (with distinct values and each with an associated ID) where the
similarity is believed to be "sparse:'That is, any two arbitrarily selected documents are very likely to
have similarity O. Design an algorithm that returns a list of pairs of document IDs and the associated
similarity.
Print only the pairs with similarity greater than 0. Empty documents should not be printed at all. For
simplicity, you may assume each document is represented as an array of distinct integers.
EXAMPLE
Input:
13: {14, 15, 100, 9, 3}
16: {32, 1, 9, 3, 5}
19: {15, 29, 2, 6, 8, 7}
24: {7, 10}
Output:
ID1, ID2 : SIMILARITY  
13, 19 :  0.1
13, 16 : 0.25
19, 24  : 0.14285714285714285


--**-----

-- MySQL Script generated by MySQL Workbench
-- Sat Dec  7 01:01:03 2019
-- Model: New Model    Version: 1.0
-- MySQL Workbench Forward Engineering

SET @OLD_UNIQUE_CHECKS=@@UNIQUE_CHECKS, UNIQUE_CHECKS=0;
SET @OLD_FOREIGN_KEY_CHECKS=@@FOREIGN_KEY_CHECKS, FOREIGN_KEY_CHECKS=0;
SET @OLD_SQL_MODE=@@SQL_MODE, SQL_MODE='ONLY_FULL_GROUP_BY,STRICT_TRANS_TABLES,NO_ZERO_IN_DATE,NO_ZERO_DATE,ERROR_FOR_DIVISION_BY_ZERO,NO_ENGINE_SUBSTITUTION';

-- -----------------------------------------------------
-- Schema mydb
-- -----------------------------------------------------
SHOW WARNINGS;
-- -----------------------------------------------------
-- Schema ctci
-- -----------------------------------------------------
DROP SCHEMA IF EXISTS `ctci` ;

-- -----------------------------------------------------
-- Schema ctci
-- -----------------------------------------------------
CREATE SCHEMA IF NOT EXISTS `ctci` DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci ;
SHOW WARNINGS;
USE `ctci` ;

-- -----------------------------------------------------
-- Table `Apartments`
-- -----------------------------------------------------
DROP TABLE IF EXISTS `Apartments` ;

SHOW WARNINGS;
CREATE TABLE IF NOT EXISTS `Apartments` (
  `apartmentID` INT(11) NOT NULL,
  `unitNumber` VARCHAR(45) NULL DEFAULT NULL,
  `buildingID` INT(11) NULL DEFAULT NULL,
  PRIMARY KEY (`apartmentID`))
ENGINE = InnoDB
DEFAULT CHARACTER SET = utf8mb4
COLLATE = utf8mb4_0900_ai_ci;

SHOW WARNINGS;

-- -----------------------------------------------------
-- Table `AptTenant`
-- -----------------------------------------------------
DROP TABLE IF EXISTS `AptTenant` ;

SHOW WARNINGS;
CREATE TABLE IF NOT EXISTS `AptTenant` (
  `apartmentID` INT(11) NOT NULL,
  `tenantID` INT(11) NULL DEFAULT NULL,
  PRIMARY KEY (`apartmentID`))
ENGINE = InnoDB
DEFAULT CHARACTER SET = utf8mb4
COLLATE = utf8mb4_0900_ai_ci;

SHOW WARNINGS;

-- -----------------------------------------------------
-- Table `Buildings`
-- -----------------------------------------------------
DROP TABLE IF EXISTS `Buildings` ;

SHOW WARNINGS;
CREATE TABLE IF NOT EXISTS `Buildings` (
  `buildingID` INT(11) NOT NULL,
  `complexID` INT(11) NULL DEFAULT NULL,
  `buildingName` VARCHAR(45) NULL DEFAULT NULL,
  `address` VARCHAR(45) NULL DEFAULT NULL,
  PRIMARY KEY (`buildingID`))
ENGINE = InnoDB
DEFAULT CHARACTER SET = utf8mb4
COLLATE = utf8mb4_0900_ai_ci;

SHOW WARNINGS;

-- -----------------------------------------------------
-- Table `Complexes`
-- -----------------------------------------------------
DROP TABLE IF EXISTS `Complexes` ;

SHOW WARNINGS;
CREATE TABLE IF NOT EXISTS `Complexes` (
  `complexID` INT(11) NOT NULL,
  `complexName` VARCHAR(45) NULL DEFAULT NULL,
  PRIMARY KEY (`complexID`))
ENGINE = InnoDB
DEFAULT CHARACTER SET = utf8mb4
COLLATE = utf8mb4_0900_ai_ci;

SHOW WARNINGS;

-- -----------------------------------------------------
-- Table `Requests`
-- -----------------------------------------------------
DROP TABLE IF EXISTS `Requests` ;

SHOW WARNINGS;
CREATE TABLE IF NOT EXISTS `Requests` (
  `requestID` INT(11) NOT NULL,
  `apartmentID` INT(11) NULL DEFAULT NULL,
  `description` VARCHAR(45) NULL DEFAULT NULL,
  `status` VARCHAR(45) NULL DEFAULT NULL,
  PRIMARY KEY (`requestID`))
ENGINE = InnoDB
DEFAULT CHARACTER SET = utf8mb4
COLLATE = utf8mb4_0900_ai_ci;

SHOW WARNINGS;

-- -----------------------------------------------------
-- Table `Tenants`
-- -----------------------------------------------------
DROP TABLE IF EXISTS `Tenants` ;

SHOW WARNINGS;
CREATE TABLE IF NOT EXISTS `Tenants` (
  `tenantID` INT(11) NOT NULL,
  `tenantName` VARCHAR(45) NULL DEFAULT NULL,
  PRIMARY KEY (`tenantID`))
ENGINE = InnoDB
DEFAULT CHARACTER SET = utf8mb4
COLLATE = utf8mb4_0900_ai_ci;

SHOW WARNINGS;

SET SQL_MODE=@OLD_SQL_MODE;
SET FOREIGN_KEY_CHECKS=@OLD_FOREIGN_KEY_CHECKS;
SET UNIQUE_CHECKS=@OLD_UNIQUE_CHECKS;




