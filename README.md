# OpenMP-Strictly-Diagonally-Dominant
##### More specifically, for a user-given number of threads:

1. The program checks if the A\[N]x\[N] matrix given by the user is [strictly diagonally dominant](https://en.wikipedia.org/wiki/Diagonally_dominant_matrix "wiki") or not
2. If so, it searches for the **max** abs element of the main diagonal of A matrix and prints it
3. Based on **max**, a new matrix A\[N]x\[N] is being created, where:
* `B[i][j] = max–abs(A[i][j]), i!=j`
* `B[i][j] = max, i==j`
4. On _B_ matrix, the **min** element along with its row and column gets found and printed

##### Compiled and executed with:
* `gcc -o main main.c -fopenmp` 
* `./main`
