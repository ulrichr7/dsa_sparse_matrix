# Sparse Matrix Operations

## Author: Manzi David

This repository implements a **Sparse Matrix** class and provides various matrix operations such as **addition, subtraction, and multiplication** on sparse matrices read from text files. It is designed to efficiently manage large matrices with predominantly zero elements by storing only the non-zero entries.

## Features

### SparseMatrix Class
- Handles sparse matrices efficiently.
- Supports reading and writing matrices from text files.
- Allows getting and setting matrix elements.

### Matrix Operations
- **Addition**: Adds two sparse matrices.
- **Subtraction**: Subtracts one sparse matrix from another.
- **Multiplication**: Multiplies two sparse matrices.

### File Handling
- Reads sparse matrices from structured text files.
- Saves computed results to output files.

### User Interaction
- Provides a simple interface to select matrices and perform operations.

## Installation
Clone the repository:

```bash
git clone https://github.com/DLOADIN/DSA_MATRIX_ASSIGNMENT/
```

Navigate to the project directory:

```bash
cd dsa/sparse_matrix/code/src
```

## Usage

### Running the Program
To execute the script, run:

```bash
python sparse_matrix_operations.py
```

### Input File Format
Matrix files should be placed in a folder named `sample_inputs/` and should follow this format:

```
num_rows = <value>
num_cols = <value>
(row, col, value)
```

#### Example (matrix1.txt):
```
num_rows = 3
num_cols = 3
(0,0,1)
(1,2,5)
(2,1,3)
```

## Operations
Once the script is running, users can choose from the following operations:

1. **Addition** - Adds two matrices.
2. **Subtraction** - Subtracts one matrix from another.
3. **Multiplication** - Multiplies two matrices.

After selecting an operation, the user will choose matrices from available files. The result will be printed to the console and saved in an output file.

### Example Usage
Performing matrix addition:
1. Select `Addition` from the operation menu.
2. Choose two matrices from the available list.
3. The result will be displayed and saved as `result_addition.txt`.

### Output Files
- **result_addition.txt** - Stores the result of matrix addition.
- **result_subtraction.txt** - Stores the result of matrix subtraction.
- **result_multiplication.txt** - Stores the result of matrix multiplication.

## Code Example
Below is an example of creating and using the `SparseMatrix` class:

```python
# Import SparseMatrix class
from sparse_matrix_operations import SparseMatrix

# Load matrices from files
matrix1 = SparseMatrix(matrix_file_path="matrix1.txt")
matrix2 = SparseMatrix(matrix_file_path="matrix2.txt")

# Perform addition
result = matrix1 + matrix2
print(result)
```

## Contributing
Contributions are welcome! Feel free to fork the repository, create a branch, and submit a pull request.

---
For more details, visit the repository: [GitHub - DLOADIN/DSA_MATRIX_ASSIGNMENT](https://github.com/DLOADIN/DSA_MATRIX_ASSIGNMENT/)

