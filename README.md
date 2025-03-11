# **Prime Number Generator and Checker**

## **Overview**
This project implements an **optimized prime number checker** and a **prime number generator** using Python. The program determines whether a given number is prime and efficiently generates a list of prime numbers up to a specified limit.

## **Features**
- **Prime Number Checker**: Uses the **6k ± 1 optimization** to check if a number is prime efficiently.
- **Prime Number Generator**: Implements the **Sieve of Eratosthenes**, one of the fastest algorithms for generating prime numbers.
- **Optimized Performance**: Reduces unnecessary computations, making it suitable for handling large numbers.

## **Problem Statement**
Prime numbers are crucial in mathematics and computing, especially in fields like cryptography and security. This project addresses the challenge of **efficiently checking for prime numbers and generating them within a given range**. A naive approach using trial division becomes inefficient for large numbers, so **optimized algorithms** are implemented to enhance computational efficiency.

## **Methodology**
### **Prime Number Checker (`is_prime(n)`)**
- Eliminates small cases (numbers ≤1 are not prime, and 2 & 3 are prime).
- Uses **6k ± 1 optimization**, reducing the number of divisibility checks.
- Time complexity: **O(√n)**.

### **Prime Number Generator (`generate_primes(limit)`)**
- Uses the **Sieve of Eratosthenes** to efficiently generate primes up to a given limit.
- Initializes a boolean list to track prime numbers.
- Time complexity: **O(n log log n)**, making it significantly faster than checking each number individually.

## **Installation & Usage**
### **Prerequisites**
Ensure you have **Python 3** installed on your system.

### **Running the Program**
1. Clone or download the repository.
2. Run the script in a Python environment:
   ```bash
   python prime_number_checker.py
   ```
3. Enter a number to check if it's prime.
4. Enter a limit to generate all prime numbers up to that number.

### **Example Usage**
#### **Checking if a number is prime:**
```
Enter a number to check if it's prime: 17  
17 is a prime number.
```

#### **Generating prime numbers up to a limit:**
```
Enter the limit to generate prime numbers: 30  
Prime numbers up to 30: [2, 3, 5, 7, 11, 13, 17, 19, 23, 29]
```

## **Applications**
- **Cryptography & Security**: Used in encryption algorithms like RSA.
- **Mathematical Computations**: Helps in number theory and factorization problems.
- **Optimization Algorithms**: Useful in computational mathematics and machine learning.

## **References**
1. Cormen, T. H., Leiserson, C. E., Rivest, R. L., & Stein, C. (2009). *Introduction to Algorithms*.
2. Python Documentation: [https://docs.python.org](https://docs.python.org)
3. Knuth, D. E. (1998). *The Art of Computer Programming, Volume 2: Seminumerical Algorithms*.

## **License**
This project is open-source and available under the MIT License.
