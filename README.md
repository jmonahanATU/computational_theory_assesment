# Computational_theory_Assesment

# Computational Theory Tasks

## What This Is
This is my work for the Computational Theory class at ATU for 2024/2025. I solved 8 different tasks that explore computer science ideas.

## Main Files
- `tasks.ipynb`: This is where all my solutions are
- `README.md`: This file that explains what I did

## What Each Task Is About

### Task 1: Binary Representations
I wrote code that works with bits (0s and 1s):
- Moving bits left (`rotl`)
- Moving bits right (`rotr`)
- Picking bits based on conditions (`ch`)
- Taking a "vote" among bits (`maj`)

I showed how each one works with examples.

### Task 2: Hash Functions
I took a hash function from the C programming example and made it work in Python.

```python
def hash_string(s):
    hashval = 0
    for char in s:
        hashval = ord(char) + 31 * hashval
    return hashval % 101
```

I explained why the numbers 31 and 101 are important.

### Task 3: SHA256 Padding
I wrote code that adds padding to a file to prepare it for SHA256 hashing:
- Adding a "1" bit
- Then adding enough "0" bits
- Finishing with the length of the original file

I tested it with the example `"abc"` to make sure it works.

### Task 4: Prime Numbers
I found the first 100 prime numbers using two different methods:
1. **Sieve of Eratosthenes**: A faster method that crosses out non-prime numbers  
2. **Trial Division**: A simpler method that checks each number individually

I compared how fast each method works.

### Task 5: Square Root Bits
I found the first 32 bits after the decimal point in the square roots of the first 100 prime numbers. For this I:
- Generated prime numbers
- Calculated their square roots
- Converted the decimal parts to binary

I showed all the results in a table.

### Task 6: Proof of Work
I found English words whose SHA256 hashes start with the most zero bits. This is similar to how Bitcoin mining works. I:
- Processed a dictionary of English words
- Calculated their SHA256 hashes
- Counted leading zeros in each hash
- Ranked the words by their zero counts

### Task 7: Turing Machine
I designed a simple computer (Turing Machine) that adds 1 to a binary number:
- It starts at the leftmost digit
- It follows simple rules to add 1
- It handles carrying over (like when `1 + 1 = 10` in binary)

I showed how it works step by step with examples.

### Task 8: Bubble Sort Analysis
I studied how many comparisons bubble sort needs:
- I wrote bubble sort with a counter
- I tested all 120 possible arrangements of the list `[1, 2, 3, 4, 5]`
- I recorded how many comparisons each arrangement needed
- I analyzed the results to understand bubble sort's efficiency

## Tools I Used
- Python programming language
- Jupyter notebooks
- Basic libraries like `math`, `numpy`, and `hashlib`

## How to Run My Code
1. Make sure Python is installed
2. Open `tasks.ipynb` in Jupyter
3. Run the cells in order from top to bottom

## What I Learned
Through these tasks, I learned about:
- How computers work with binary numbers
- Different ways to solve the same problem
- How to measure how efficient algorithms are
- Basic concepts in cryptography and computing theory
- 

## References

- NIST FIPS 180-4 Specification. For SHA-256 padding details in Task 3.
- Atwood, E. (2019). "Prime Number Generation: Comparing Algorithms" for the Sieve of Eratosthenes implementation.

- Stack Overflow. ["Generating Permutations using Python's Itertools."](https://stackoverflow.com/a/104436)
- Stack Overflow. ["Appending bits to the start of a binary number."](https://stackoverflow.com/a/51678298)
- Python Documentation. ["ord() function reference."](https://docs.python.org/3.4/library/functions.html?highlight=ord#ord)
- Stack Overflow. ["Open file with encoding."](https://stackoverflow.com/a/49375134)
- GeeksforGeeks. ["Splitting an array into even-sized chunks."](https://www.geeksforgeeks.org/break-list-chunks-size-n-python/)
- CP-Algorithms. ["Sieve of Eratosthenes."](https://cp-algorithms.com/algebra/sieve-of-eratosthenes.html)
- W3Schools. ["Bubble Sort Algorithm Explanation."](https://www.w3schools.com/dsa/dsa_algo_bubblesort.php)
- GeeksforGeeks. ["Sieve of Atkin for Prime Generation."](https://www.geeksforgeeks.org/sieve-of-atkin/)
- Back, A. (2002). *"HashCash - A Denial of Service Counter-Measure."* [PDF](http://www.hashcash.org/hashcash.pdf)
- W3Schools. ["Bubble Sort Time Complexity Analysis."](https://www.w3schools.com/dsa/dsa_timecomplexity_bblsort.php)


