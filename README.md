Sparse Matrix Operations
This project implements a Sparse Matrix class and several matrix operations (addition, subtraction, multiplication) on sparse matrices read from text files. It is designed to efficiently handle large matrices with mostly zero elements, storing only the non-zero entries.

Features
SparseMatrix Class: Handles sparse matrices, including reading from files, getting and setting elements, and performing matrix operations.
Matrix Operations: Supports matrix addition, subtraction, and multiplication.
File Handling: Read and write sparse matrices to text files.
User Interaction: Allows users to choose matrices and perform operations through a simple interface.
Requirements
Python 3.x
Installation
Clone the repository to your local machine:

bash
Copy
Edit
git clone https://github.com/yourusername/sparse-matrix-operations.git
Navigate to the project directory:

bash
Copy
Edit
cd sparse-matrix-operations
Usage
Running the Program
To run the program, simply execute the script:

bash
Copy
Edit
python sparse_matrix_operations.py
Input Files
The program expects the matrix files to be stored in a folder named sample_inputs/. Each matrix file should follow this format:

The first line should contain the number of rows: num_rows = <value>
The second line should contain the number of columns: num_cols = <value>
The subsequent lines should represent non-zero elements in the format (row, col, value)
Example matrix file (matrix1.txt):

makefile
Copy
Edit
num_rows = 3
num_cols = 3
(0,0,1)
(1,2,5)
(2,1,3)
Operations
After running the script, you'll be prompted to select an operation:

Addition: Add two matrices.
Subtraction: Subtract one matrix from another.
Multiplication: Multiply two matrices.
After selecting an operation, you'll be asked to choose the matrices from available files. The result of the operation will be printed to the console and saved in a file.

Example
To perform matrix addition:

Choose Addition from the operation menu.
Select two matrices from the list.
The result will be displayed, and the sum will be saved as result_addition.txt.
Matrix Files
To list matrix files in the sample_inputs/ directory:

bash
Copy
Edit
matrix1.txt
matrix2.txt
Output Files
The result of addition will be saved in result_addition.txt.
The result of subtraction will be saved in result_subtraction.txt.
The result of multiplication will be saved in result_multiplication.txt.
Example Code
python
Copy
Edit
# Example of creating and using SparseMatrix
matrix1 = SparseMatrix(matrix_file_path="matrix1.txt")
matrix2 = SparseMatrix(matrix_file_path="matrix2.txt")

# Perform addition
result = matrix1 + matrix2
print(result)




