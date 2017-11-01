# Samsung Research Institute Interview Questions
* [Coding Round Questions](#coding)
* [Technical Interview Questions](#tech)
   * [Data Structures and Algorithms](#dsalg)
   * [DBMS](#dbms)
   * [Operating System](#os)
   * [Miscellaneous](#misc)
* [References](#ref)
____
<b name="coding">Coding round questions</b><br/>
- Company S has developed an industrial endoscope available to explore inner part of the decrepit water pipes.
  It is possible to explore the inner part of the pipes putting the endoscope in a certain part of the pipe.
  The endoscope can be moved in the pipe only. Meanwhile, when the pipes are connected to each other, if the length of the endoscope is long enough to explore ,then it is able to inspect the connected pipes. However, we cannot observe every pipe because the length of endoscope is limited.

  When the map of the ground water pipe, the location where the endoscope to out in, and the length of the endoscope is given, calculate the number of pipe which are available to explore. Length of endoscope means the range upto which endoscope can explore. There are seven kind of pipes, and description for each pipe are shown below:
  
  
 | S.No | Pipe           | Connected to  |
 | -----|:-------------: | -------------:|
 | 1    | ![](https://github.com/rishabh115/InterviewQuestions/raw/master/Samsung/res/1.png ) | Up, Down, Left, Right |
 | 2    | ![](https://github.com/rishabh115/InterviewQuestions/raw/master/Samsung/res/2.png ) | Up, Down              |
 | 3    | ![](https://github.com/rishabh115/InterviewQuestions/raw/master/Samsung/res/3.png ) | Left, Right           |
 | 4    | ![](https://github.com/rishabh115/InterviewQuestions/raw/master/Samsung/res/4.png ) | Up, Right             |
 | 5    | ![](https://github.com/rishabh115/InterviewQuestions/raw/master/Samsung/res/5.png ) | Down, Right           |
 | 6    | ![](https://github.com/rishabh115/InterviewQuestions/raw/master/Samsung/res/6.png ) | Down, Left            |
 | 7    | ![](https://github.com/rishabh115/InterviewQuestions/raw/master/Samsung/res/7.png ) | Up, Left              |

  When the map of the ground water pipe, the location where the endoscope to out in, and the length of the endoscope is given, calculate the number of pipe which are available to explore. Length of endoscope means the range upto which endoscope can explore.
   #### Input
   In the first line, T, the number of total test cases is given. From the second line, T test cases are given. In the first line of each test case, N, the height of the map of the ground water pipes, M, the width, R, the vertical location of the water pipe where to put in the endoscope, C, the horizontal location of it, and the length of the endoscope L are given. In the following N lines information of the map of ground water pipe is given. Each line has M numbers. Each number (from 1 to 7) means the type of water pipe for that point. 0 means there is no water pipe buried in that place.

   #### Output
   Print the respective answer for T test cases in total for T lines. The answer is the number of water pipes which is available to observe using the endoscope.

   #### Constraints
   1≤ T ≤100

   1≤ N, M ≤50

   0≤ X < N

   0≤ Y < M

   1≤ L ≤ 20
         
- Given a graph print either of the set of the vertices that are colored with the same color. And if the graph is not bipartite print “-1”. Test cases also included the cases when a graph is not connected.
- You’ll be given a grid as below:
   ```
                          0 1 0 2 0 --> Non highlighted part
                          0 2 2 2 1
                          0 2 1 1 1
                          1 0 1 0 0
                          0 0 1 2 2
                          1 1 0 0 1
                          x x S x x  -->highlighted yellow
   ```
     In the grid above,     
  1: This cell has a coin.  
  2: This cell has an enemy.    
  0: It contains nothing.     
  The highlighted(yellow) zone is the control zone. S is a spaceship that we need to control so that we can get maximum coins.      
  Now, S’s initial position will be at the center and we can only move it right or left by one cell or do not move.
  At each time, the non-highlighted part of the grid will move down by one unit.    
  We can also use a bomb but only once. If we use that, all the enemies in the 5×5 region above the control zone will be killed.  
  If we use a bomb at the very beginning, the grid will look like this:
 ```
 0 1 0 2 0  --> Non highlighted part
 0 0 0 0 1
 0 0 1 1 1
 1 0 1 0 0
 0 0 1 0 0
 1 1 0 0 1
 x x S x x  --> highlighted yellow
 ```
   As soon as, the spaceship encounters an enemy or the entire grid has come down, the game ends.     
  For example,    
  At the very first instance, if we want to collect a coin we should move left **( coins=1)**. This is because when the grid comes down by 1 unit we have a coin on the second position and by moving left we can collect that coin. Next, we should move right to collect another coin **( coins=2)** .
  After this, remain at the same position **( coins=4)**.
  This is the current situation after collecting 4 coins.
 ```
 0 1 0 2 0                0 1 0 0 0
0 2 2 2 1 -->after using 0 0 0 0 1
x x S x x -->bomb        x x S x x
 ```
 Now, we can use the bomb to get out of this situation. After this, we can collect at most 1 coin. So maximum coins=5.
- A Research team want to establish a research center in a region where they found some rare-elements.They want to make it closest to all the rare-elements as close as possible so that they can reduce overall cost of research over there.It is given that all the rare-element’s location is connected by roads.It is also given that Research Center can only be build on road.Team decided to assign this task to a coder.If you feel you have that much potential.                   
Here is the Task :- Find the shortest of the longest distance of research center from given locations of rare-elements.     
locations are given in the matrix cell form where 1 represents roads and 0 no road..
number of rare-element and their location was also given(number<=5)
and order of square matrix was less than equal to (20).
- Given a Binary Tree where each node has positive and negative values. Convert this to a tree where each node contains the sum of the left and right sub trees in the original tree. The values of leaf nodes are changed to 0.
- Write a function that calculates the day of the week for any particular date in the past or future. A typical application is to calculate the day of the week on which someone was born or some other special event occurred.
- Given a Binary Tree, write a function that returns the size of the largest subtree which is also a Binary Search Tree (BST). If the complete Binary Tree is BST, then return the size of whole tree.
- You are given an array of integers which represents positions available and an integer c(cows).   
Now you have to choose c positions such that minimum difference between cows is maximized.
```
For example,
1 3 5 8 10
c=3
output: 4
1 5 10
 ```
- Given a Binary Tree and a node x in it, find distance of the closest leaf to x in Binary Tree. If given node itself is a leaf, then distance is 0.
- Given random points in a 2-D plane, construct a convex polygon with minimum area of covering and which encompasses all the given points.
- Given a graph, find out if it can be colored using 2 colors. If Yes, print numbers of vertices with any one of the colour, followed by such vertices in sorted order. If No just print -1
- Given a 2 D matrix where 1 represent the places where the frog can jump and 0 represent the empty spaces, the frog can move freely in horizontal direction (on 1’s only) without incurring any cost (jump).A vertical jump from a given point of the matrix to other point on the matrix can be taken (on 1’s only) with cost as the number of jumps taken.        
Given a source and destination, the frog has to reach the destination minimizing the cost (jump)
- Given a directed graph. Check whether a graph contain a cycle or not.
- Given a level K , you have to find out the sum of data of all the nodes at level K in a binary tree.
Input is given as:  
     ```       
     (P(C()())(C()()))
     P is for Parent, C is for child.
     if parent has one child : (P(C()())())
     if parent has no child : (P()())
     ```
- A company sells its products with a unique serial number on it. Company has has found that there are some products that don’t sell well which are identified to have ominous numbers in the serial number of the product. So if a serial number of the product contains atmost ’k’ ominous number then it won’t sell.
   Given a range form s to e, you need to find number of products that would sell, leaving out the products that contains atmost ’k’ ominous numbers. 
   
 ``
 Input: First line contains the number of test cases, followed buy the range s to e, 1     
 ``
- You are given N unique numbers a1<a2<a3<...an. Find out the count of all possible binary search tress that can be constructed using these numbers.
For example with 3 elements 1,2,3 there are 5 possible BST and for 1,2,3,4 there are 14 BST.

- Given an NxM (N rows and M columns) integer matrix with non-negative values (0..MAX_INT inclusive). What is the maximum sum from going top left (0, 0) to bottom right (N-1, M-1) ? The condition is that when you're at point (p, q), you can only move to either right (p, q+1) or down (p+1, q).
- Mr. Kim has to deliver refrigerators to N customers. From the office, he is going to visit all the customers and then return to his home. Each location of the office, his home, and the customers is given in the form of integer coordinates (x,y) (0≤x≤100, 0≤y≤100) . The distance between two arbitrary locations (x1, y1) and (x2, y2) is computed by |x1-x2| + |y1-y2|, where |x| denotes the absolute value of x; for instance, |3|=|-3|=3. The locations of the office, his home, and the customers are all distinct. You should plan an optimal way to visit all the N customers and return to his among all the possibilities.       
You are given the locations of the office, Mr. Kim’s home, and the customers; the number of the customers is in the range of 5 to 10.
Write a program that, starting at the office, finds a (the) shortest path visiting all the customers and returning to his home. Your program only have to report the distance of a (the) shortest path.

    **Constraints**

    5≤N≤10. Each location (x,y) is in a bounded grid, 0≤x≤100, 0≤y≤100, and x, y are integers.

    **Input**

    You are given 10 test cases. Each test case consists of two lines; the first line has N, the number of the customers, and the following line enumerates the locations of the office, Mr. Kim’s home, and the customers in sequence. Each location consists of the coordinates (x,y), which is reprensented by ‘x y’.

    **Output**

    Output the 10 answers in 10 lines. Each line outputs the distance of a (the) shortest path. Each line looks like ‘#x answer’ where x is the index of a test case. ‘#x’ and ‘answer’ are separated by a space.


    I/O Example

    Input (20 lines in total. In the first test case, the locations of the office and the home are (0, 0) and (100, 100) respectively, and the locations of the customers are (70, 40), (30, 10), (10, 5), (90, 70), (50, 20).)


    5 ← Starting test case #1

    0 0 100 100 70 40 30 10 10 5 90 70 50 20

    6 ← Starting test case #2

    88 81 85 80 19 22 31 15 27 29 30 10 20 26 5 14

    10 ← Starting test case #3

    39 9 97 61 35 93 62 64 96 39 36 36 9 59 59 96 61 7 64 43 43 58 1 36

    Output (10 lines in total)

    #1 200

    #2 304

    #3 366

- Given a graph question. We have to find the loop in the graph if it exist and print the nodes of the loop in sorted order.

- You are given an old touch smartphone numbers having dial pad and calculator app.
The goal is to type a number on dialpad.
Calculator have 1-9 and +, -, \* , /, = as operations. But as phone is old, some of the numbers and some operations can't be touched.
But you can always make a number using other numbers and operations. There could be multiple ways of making a number. You have to find minimum operation for making a number.  
For ex: lets say 1,4,6,7,8,9 works and +,-,* works.
2,3,5 and / doesn't work.     
If you have to type 18-> 2 operations. (Each touch is considered an operation).    
If you have to type 5 -> '1+4=' that requires 4 operations. There could be other ways to make '5'.  
  The goal is to find minimum operations.

- There are N pots. Every pots has some water in it. They may be partially filled . Every pot is associated with overflow number O which tell how many minimum no. of stones required for that pot to overflow. The crow know O1 to On(overflow no. for all the pots). Crow wants some K pots to be overflow. So the task is minimum number of stones he can make K pots overflow in worst case.

  Array of overflow no--. {1,...,On}   
  Number of pots--n     
  No of pots to overflow-- k

  Let say two pots are there with overflow no.s {5,58}, and crow has to overflow one pot(k=1). So crow will put 5 stones in pot with overflow no.(58), it will not overflow, then he will put in pot with overflow no.(5), hence the total no. of stones to make overflow one pot is=10.

- You are given 2 convex hulls. Find all the common points that lie in the intersection of these 2 convex hulls.

- There is one spaceship. X and Y co-odinate of source of spaceship and destination spaceship is given. There are N number of warmholes; each warmhole has 5 values.
First 2 values are starting co-ordinate of warmhole and after that value no. 3 and 4 represents ending co-ordinate of warmhole and last 5th value is represents cost to pass through this warmhole. Now these warmholes are bi-directional.
Now the to go from (x1,y1) to (x2,y2) is abs(x1-x2)+abs(y1-y2).
The main problem here is to find minimum distance to reach spaceship from source to destination co-ordinate using any number of warm-hole. It is ok if you wont use any warmhole.
- There is an island surrounded by oil mines. You will be given n companies and m oil mines having values. You have to distribute the mines to "n" companies in fair manner. Remember the companies can have oil mines adjacent to each other and not in between of each others.After distributing them compute the difference of oil mines from the company getting highest and company getting lowest. This number should be minimum.(then only the distribution can be termed as fair).


        Example
        Input
        2
        2 4
        6 13 10 2
        2 4
        6 10 13 2

        output
        5
        1

 -  There is a n x n matrix with only 0s & 1s. Letters are formed using 1 and 0.
      For eg.-
      
              
              
                   U is 1 0 1,  V is 1 0 1
                        1 0 1        1 0 1
                        1 1 1        0 1 0  
                        
              
              
    Likewise there are 6 letters and they can rotated in 90, 180, 270, 360 degree. And if there is a letter, the next column would be filled with 0.
                Eg. 
                
                
                
                    V- 1 0 1 0
                       1 0 1 0
                       0 1 0 0
                       
                
                
    So we have to count the number of each letter in the matrix.
    
- There is a maze that has one entrance and one exit.
Jewels are placed in passages of the maze.
You want to pick up the jewels after getting into the maze through the entrance and before getting out of it through the exit.
You want to get as many jewels as possible, but you don’t want to take the same passage you used once.

  When locations of a maze and jewels are given,
find out the greatest number of jewels you can get without taking the same passage twice, and the path taken in this case.

 ![](https://github.com/rishabh115/InterviewQuestions/blob/master/Samsung/res/jewel.jpg?raw=true)
 #### Input
  There can be more than one test case in the input file. The first line has T, the number of test cases.
  Then the totally T test cases are provided in the following lines (T ≤ 10 ).

  In each test case,
  In the first line, the size of the maze N (1 ≤ N ≤ 10) is given. The maze is N×N square-shaped.
  From the second line through N lines, information of the maze is given.
  “0” means a passage, “1” means a wall, and “2” means a location of a jewel.
  The entrance is located on the upper-most left passage and the exit is located on the lower-most right passage.
  There is no case where the path from the entrance to the exit doesn’t exist.

  #### Output
  From the first line through N lines, mark the path with 3 and output it.
  In N+1 line, output the greatest number of jewels that can be picked up.
  Each test case must be output separately as a empty.
    



----
<b name="tech">Technical Interview Questions</b>
<br/>
<i><u name="dsalg">Data Structures and Algorithms</u></i>
- Write the code of heap sort and complexity in different cases.
- Implement Kadane's Algorithm.
- Kahn's algorithm for topological sorting.
- Which DS is used to manage files and folder in your mobile?
- Write code for Dijkstra Algorithm.
- Find the kth minimum element into binary search.
- What is memory leak? How to avoid it?
- Write a program to create circular queue?  
- Detect and remove loop in linked list.
- Design LRU data structure.
- Zigzag traversal between two singly linked list.
- There is a N*M matrix where each row is sorted. Find the kth largest element in matrix?
- Print sum of all prime numbers within a given range.
- Find the largest and second largest element in array. Give 4 different approaches.
-  Given two polynomials as linked lists, return a linked list which represents the product of two polynomials.
- What is the difference between dynamic programming and divide and conquer?
- Given two polynomials represented by two arrays, write a function that multiplies given two polynomials.
- What are the disadvantages of stack.
- Write a program to find when we get stack overflow if we are using recursive functions.
<br/><br/>
<i><u name="dbms">DBMS</u></i>

- What is view in DBMS?
- What is Indexing?

<br/>
<br/>
<i><u name="os">Operating System</u></i>

- What is page fault and why it occurs?
- What is virtual memory?
- What is Demand Paging?
- Explain Semaphore.
- While context switching takes place what is stored on stack and heap.
- Write code for Producer-Consumer Problem.
- What is Swap In and Swap Out?
- Differentiate between Starvation and Aging.
- Explain the page replacement Algorithm LRU.
- What is Inter process communication ,types and which one is fast and why?
- What is fragmentation? Define external fragmentation.
- Calculate the number of processes generated using N fork() statements?
- Due to priority of process, what type of problem occurs in priority scheduling?
- What is real time OS.
- Difference between preemptive and non- preemptive algorithms.
- If time slice is greater than the execution time of largest execution time process than round robin acts as...?
- There is a file and 5 processes. How can you grant access so that
only 2 process can write to file and 1 can read file at a time .
- Stack pointer vs Frame pointer.
<br/>
<i><u name="misc">Miscellaneous</u></i>

- Explain and give an example of a function pointer. Write function pointer for a function that takes an integer as a parameter and returns character.
- Implement you own strcat() function. Dont use string header.
- Difference between TCP and UDP.
- What is Inline functions?
- Write a program to allocate a 3D-array dynamically.
- Write your own typedef operator.
- What is meant by Early binding and late binding.
- State various protocols in various layers of TCP/IP.
- Create a pointer that can point to an array of integers.
- Explain client server architecture.
- What is  L-value and R-value reference?
- State various principles of OOPS.
- Define MFC COM and DCOM.
- What is meant by Big and Small Endian? How would you know that Machine code is Big or Small Endian?
- What is friend class and function in C++?
- What is Virtual Function in C++?
- Full form of conio.
- Describe Java's garbage collection.
- Explain Abstract and pure Virtual function in detail.
- What is the difference between a static and const variable?
- Do namespaces interact? if yes, how? if no, why not?
- Define Scheduling. Which data structure is used in scheduling?
- Where are the local, global, static, auto, register, extern, const, volatile variables stored?
- What is a virtual destructor? Explain the use of it - C++.
- What is a void pointer, a smart pointer, a wild pointer, a null pointer, and a dangling pointer? In what cases are they used?
- What is the difference between a deep copy and a shallow copy?
- Explain Diamond problem in C++.
- What is segmentation fault?
- Implement 3 stacks using 1 array.
- Explain MultiLevel inheritance.
- Memory layout of C program.
- What is structure padding ?
- What is function pointer?
- There are some exceptions that cannot be caught by try catch. How to catch such exceptions? Can we prevent our program to crash if we are not able to catch such exceptions.
- What is name mangling, and how does it work?
- What does malloc(0) return?