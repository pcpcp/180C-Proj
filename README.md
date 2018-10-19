# 180C-Proj
Sudoku Solution Multithreading Validator

The topic we choose is to implement a sudoku solution multithreading validator.
A sudoku is a combinatorial number placement puzzle. The aim is to fill the 9 x 9 grid in each column and row, and each of the nine 3 x 3 subgrids.
Each column, row and subgrid must contain all of the digits from 1 through 9. 
The approach suggested by the textbook is to create eleven threads, each realizes the following specification:
1.   A thread checks each column contains the digits 1 through 9
2.   A thread checks each row contains the digits 1 through 9
3.   Nine threads check each 3 x 3 subgrids contains the digits 1 through 9

The potential problem of this approach is that it only has one thread checking columns, and one thread checking rows. 
Since the multithreaded system can utilize the multiprocessors on the CPU, there is no harm to use more threads in our approach. 
We will generate one thread for each column, and one thread for each row.
Therefore, we will have total of 27 threads to validate the sudoku concurrently. 
The final delivery will be a C program implementing the pthread library. 
