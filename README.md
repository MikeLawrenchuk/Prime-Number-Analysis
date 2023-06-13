# Prime-Number-Analysis
This Python program reads a list of prime numbers from a file, and then finds pairs of primes whose last digits (when considered as strings) multiply to a certain target.
This Python program reads a list of prime numbers from a file, and then finds pairs of primes whose last digits (when considered as strings) multiply to a certain target.

## Code Description

The program consists of two main functions:

1. `read_primes_from_file(filename)`: This function reads a list of prime numbers from a file. The file should contain one prime number per line.

2. `find_prime_pairs(target_last_digit, primes)`: This function finds pairs of primes whose last digits multiply to a certain target. The primes are considered as strings, and the last digit of each prime is extracted for the multiplication.

The program reads the primes from a file, finds the pairs of primes, and then prints these pairs.

## Code Modifications

The program can be modified to consider more than one digit at the end of each prime. To do this, you would need to change the line in `find_prime_pairs` that extracts the last digit:

```python
last_digit1 = int(str(primes[i])[-1:])
last_digit2 = int(str(primes[j])[-1:])
```

You can change `-1:` to `-n:` to consider the last `n` digits, where `n` is the number of digits you want to consider.

## Output

The program prints the pairs of primes that it finds. If you want to output a full list of the primes that it read from the file before it attempts to find the pairs, you can add the following line after reading the primes:

```python
print(primes)
```

This will print the list of primes.

---
