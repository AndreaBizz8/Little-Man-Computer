# Little-Man-Computer
Program to open with Little Man Computer 
As it can be clearly seen, the program will ask for an input that will move you to:

a) Fibonacci code if the input is 1
b) Greater to smaller with 3 number if the input is different than 1;
c) End of the program if the input is zero.
To understand better how every branch works, you can check the Explanation below

FIBONACCI
Fibonacci is a sequence that start from “0” zero and “1” and then the following number are the sum of the 2 preceding ones. (0-1-1-2-3-5-8-13-21-…)
As you can see Fibonacci will ask the user to insert a number that will be used to run the branch a counted amount of time.
In this case after storing the value it can co to the actual code to calculate the Fibonacci sequence or it can go to the end of the branch going then back to main start.

To keep in mind that in as the LMC has only a range of number (from -500 to 499) at the moment that calculating the program will go over 499 it will start from -500 and it will go on and on. That is why on Fibonacci we will have the correct positive number only till 377 then we will have a negative number as the sum of the 2 number before (377 and 233) is obviously bigger than 499.


THREE NUMBER GREATER TO SMALLER
For this part of the program I had to try different way to check every possible output giving 3 number.
With 3 number you can have 6 different output:
A-B-C		A-C-B		B-A-C		B-C-A-		C-A-B		C-B-A
Now that we have all the different outputs, we have to start checking every single combination. 
After checking every combination it is clear that to arrive to every output we need 2 or 3 check loop.
If I check A and B at the beginning I can have 2 result A>B or B>A in both case I will have to check A and C, but only if A>B & C>A we have output C-A-B and if B>A & C>B we will have output C-B-A.
For the other 4 possibilities we will have to create 2 more loop, in case A>B and A>C it is clear that we have to check B and C to get to the 2 output B-A-C and B-A-C. Same in case B>A and B>C we have to check A and C to get to the last 2 output B-A-C and B-C-A.
