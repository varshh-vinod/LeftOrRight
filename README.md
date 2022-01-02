# LeftOrRight
Problem Statement
    	The Very Heterogeneous State of Feudalia's army is designing a new spy robot. Currently, the robot can only accept two commands: L and R. L moves the robot one unit of distance to the left, and R moves the robot one unit to the right. A program for the robot is a sequence of commands. For a given program, its reach is the distance between the starting point and the farthest point visited during the execution of the program. For example, the reach of the program "LLLR" is 3, because after the first three steps we reach a location 3 units away from the starting point.
Unfortunately, Feudalia is world famous for the ineptitude of its public officials. Some coffee was spilled all over the program before it could be installed to the robot. Therefore, some of the commands may now be illegible. Your task is to repair the program by replacing each illegible command with an L or an R. If there are multiple ways to repair the program, you have to pick one that maximizes its reach.
You are given a String program which describes the program in its current state. The i-th character in program represents the i-th command that is executed and will be 'L', 'R' or '?' (quotes for clarity). 'L' represents a legible move left, 'R' a legible move right and '?' a command that is illegible so you can choose 'L' or 'R' in its place. Return the largest reach a repaired program can have.
 
Definition
Method signature:	int MaxDistance(String program)

Constraints
-	program will contain between 1 and 50 characters, inclusive.
-	Each character of program will be 'L', 'R' or '?' (quotes for clarity).
 
Examples

1)    	
"LLLRLRRR"
Returns: 3
All commands are legible. The reach of this program is 3: both after three steps and after five steps we are 3 units to the left of the starting location.

2)    	
"R???L"
Returns: 4
We can replace all of the question marks with a right command.

3)    	
"??????"
Returns: 6

4)    	
"LL???RRRRRRR???"
Returns: 11

5)    	
"L?L?"
Returns: 4
