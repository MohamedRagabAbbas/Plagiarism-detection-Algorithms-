# Plagiarism Detection Algorithms

This repository contains implementations of various string matching algorithms for detecting plagiarism in text documents. The supported algorithms include:

1. **Rabin-Karp Algorithm**
2. **Knuth-Morris-Pratt (KMP) Algorithm**
3. **Boyer-Moore Algorithm**
4. **Hamming Distance Brute Force Algorithm**

## Getting Started

### Prerequisites

- A C++ compiler (e.g., g++, clang)
- Text files for testing the plagiarism detection

### File Structure

- `main.cpp` - The main file containing the implementations of the algorithms and the function to test for plagiarism.
- `file1.txt`, `file2.txt`, `file3.txt` - Example database files to compare against.
- `testfile.txt` - Example test file to check for plagiarism.

### Running the Program

1. Compile the `main.cpp` file using your C++ compiler. For example:

    ```sh
    g++ main.cpp -o plagiarism_detection
    ```

2. Run the compiled program:

    ```sh
    ./plagiarism_detection
    ```

### Functionality

The program reads a test file and checks its contents against a set of database files using different string matching algorithms. The results, including the percentage of plagiarized content and the documents from which content was plagiarized, are displayed for each algorithm.

### Example Output

```sh
Rabin-Karp: 
50%
Documents from which the test file was plagiarized: 
1. file1.txt
2. file2.txt
---------------------------------------------------
Knuth-Morris-Pratt: 
40%
Documents from which the test file was plagiarized: 
1. file1.txt
---------------------------------------------------
Boyer-Moore: 
30%
Documents from which the test file was plagiarized: 
1. file2.txt
---------------------------------------------------
Hamming Distance: 
60%
Documents from which the test file was plagiarized: 
1. file1.txt
2. file3.txt
