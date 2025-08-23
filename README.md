Pseudorandon Number Generator(PRNG) is an algorithm that uses a mathematical formula to produce a sequence of numbers that appears randon 

1) Pseudorandom number generator
   •	random.seed(42) fixes the random seed so that the same numbers are produced every time the code runs (useful for testing or debugging).
•	A list comprehension generates 10 integers, each chosen randomly between 1 and 100.
•	Finally, the list is printed.


2) Blum Blum randon number Generator
•	is_prime(n): Checks if a number n is prime.
•	generate_blum_integer(): Randomly generates a Blum integer n = p × q, where p and q are prime numbers such that both are congruent to 3 (mod 4). This condition ensures security properties of BBS.
•	blum_blum_shub(seed, length, n):
o	Starts with a seed reduced modulo n.
o	Repeatedly computes:
xi+1=xi2mod  nx_{i+1} = x_i^2 \mod n 
o	Extracts the least significant bit (x % 2) at each step.
o	Collects length bits to form the pseudorandom output.
•	Usage:
o	A Blum integer n is generated.
o	A random seed is chosen.
o	The generator produces 16 pseudorandom bits.



3) Linear-congruential-Generator
This code implements a Linear Congruential Generator (LCG), a simple algorithm for generating pseudo-random numbers.
•	The function lcg(seed, a, c, m, n) generates n numbers starting from an initial seed.
•	Each new number is computed using the formula:
xi+1=(a⋅xi+c)mod  mx_{i+1} = (a \cdot x_i + c) \mod m 
•	Here:
•	a is the multiplier,
•	c is the increment,
•	m is the modulus,
•	seed is the starting value.
•	In this example, the generator produces 10 pseudo-random numbers using common LCG parameters (from Numerical Recipes).
•	The output list pseudo_random_numbers contains those generated values.

   
