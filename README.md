# Maximum-Number-Of-Handshakes-C-Program

Maximum number of handshakes in C
Here, in this section we will discuss the program for maximum number of handshakes in C. The user is asked to take a number as integer n and find out the possible number of handshakes. For example, if there are n number of people in a meeting and find the possible number of handshakes made by the person who entered the room after all were settled.

Maximum number of handshakes in C
Approach :
For the number of handshakes to be maximum, every person should hand-shake with every other person in the room

i.e. all persons present should shake hands.

For the first person, there will be N-1 people to shake hands with
For second person, there will be N -1 people available but as he has already shaken hands with the first person, there will be N-1-1 = N-2 shake-hands
For third person, there will be N-1-1-1 = N-3, and So On…
Therefore the total number of handshake   =   ( N – 1 + N – 2 +….+ 1 + 0 )   =   ( (N-1) * N ) / 2.

Algorithm
For N = 10
handshakes  =  ( (N-1) * N ) / 2  =  ( 10 x 9 )/2  =  45
Print Result
Maximum number of handshakes
While loop in C
Related Pages
Quadrants in which a given coordinate lies
 
Permutations in which n people can occupy r seats in a classroom
 
Addition of two fractions

Replace all 0’s with 1 in a given integer

Can a number be expressed as a sum of two prime numbers

C Code
Run
// C program to find the maximum number of handshakes
#include

int main()
{

    //fill the code
    int num = 10;

    int total = num * (num-1) / 2; // Combination nC2

    printf("For %d people there will be %d handshakes", num, total);

    return 0;

}
Output
For 10 people there will be 45 handshakes
