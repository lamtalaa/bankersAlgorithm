# Banker’s Algorithm for deadlock avoidance
The banker’s algorithm is a resource allocation and deadlock avoidance algorithm that tests for safety by simulating the allocation for predetermined maximum possible amounts of all resources, then check for safe state to test for possible activities, before deciding whether allocation should be allowed to continue.

How does the program work?

We start by calculating the need matrix with is equal to maximum minus available matrix, then we compare values of need and available matrices, if need is less than availabe then that instance is next on the safe sequence, if it is greater then we add allocation to available and we do the same comparison again until we check all the instances we have, this way at the end we can get the same sequence.

How to compile and run the program:

To compile the program use the following command:
gcc bankersAlgorithm.c -o bankersAlgorithm

this will generate a new object file bankersAlgorithm.o

To run the program, use the following command:
./bankersAlgorithm
