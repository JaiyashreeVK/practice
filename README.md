# practice problems
INTRODUCTORY PROBLEMS

1. WEIRD NUMBER SERIES Consider an algorithm that takes as input a positive integer n. If n is even, the algorithm divides it by two, and if n is odd, the algorithm multiplies it by three and adds one. The algorithm repeats this, until n is one. For example, the sequence for n=3 is as follows:
3→10→5→16→8→4→2→1
Your task is to simulate the execution of the algorithm for a given value of n.

solution:
I took input n value and used if else condition statements inside a while loop to get the correct answer.
IF n is even: n=n/2
ELSE IF n is odd: n=(n*3)+1
PRINT n


2.MISSING NUMBER

You are given all numbers between 1,2,…,n except one. Your task is to find the missing number.

Solution:
I was familiar with the question before, I went with the method of finding the sum of numbers till n
and subract it with sum of the given array to find the missing value.

sum=n*(n+1)/2; //sum of no.s till n
miss=sum-arr_sum; //difference between sum and array sum gives missing value


3. DNA repetition

You are given a DNA sequence: a string consisting of characters A, C, G, and T. Your task is to find the longest repetition in the sequence. This is a maximum-length substring containing only one type of character.

solutions:
I took the input string and traversed to find if current character is same as previous character, if so then i incremented the count value.
else I found the maximum count of repeated elements till that string position by comparing with previous maximum value and count. 
After finding I changed count back to 1 and repeat for rest of the string.
Outside the loop i again check max count value after reaching the end of the string to get final max lenght(count) of repeation characters in the array.


4.Incresing Array

You are given an array of n integers. You want to modify the array so that it is increasing, i.e., every element is at least as large as the previous element.
On each turn, you may increase the value of any element by one. What is the minimum number of turns required?

Solution:
I initially mistook the qn as a sorting problem but later i understood that it is not gonna get swapped in one turn but multiple turns by adding one.
I used a for loop to traverse the given array and used if else condition to check if the elements that are not in ascending order.
If the element is greater than the next element in the array, 
I calculated the difference between them(to find the number of turn it will take to swap the umbers by add 1 to the lesser element)
swaped the elements and incremented the count with the differnece value, to find the correct answer.


5.Permutations

A permutation of integers 1,2,…,n is called beautiful if there are no adjacent elements whose difference is 1.
Given n, construct a beautiful permutation if such a permutation exists.

Solutions:
It took me some time to understand this question, that's when i noticed the pattern in the output, 
it was alternative even and odd numbers, that has the differnec greater than 1.
I took the base cases where the above cannot be checked, such as 1 will be having only 1 value therefore it has 1 solution.
for n=2 and n=3, the solutions are not possible in any of the possible arrangements.
after checking the base cases, I checked for whether the number is even or odd depending on that, the value I should start and end would be different.
If n is even then i printed the even elements first and then followed by it the odd elements 
Else, if n is odd then I printed the odd first and then even numbers. such that the elements preceeding the even/odd series does not have a differnce of 1.


6. Trailing zero

Your task is to calculate the number of trailing zeros in the factorial n!.
For example, 20!=2432902008176640000 and it has 4 trailing zeros.

solution:
I was familiar with the question already, the logic i used was the prime factors that will produce a zero in the last place of a number, that is 5 and 2.
just by counting the number of 5 in the list of prime factors of the no., we can find the number of zeros in the factorial of a given number.
I Kept dividing n by powers of 5 in a for loop , and incremented count with result value because 5 is a prime factor that gives zero in the unit place.


7.Bit string

Your task is to calculate the number of bit strings of length n.
For example, if n=3, the correct answer is 8, because the possible bit strings are 000, 001, 010, 011, 100, 101, 110, and 111.

Solution:
it reminded me of the formula of binary repersentation 2^n combinations of values for n bits.
I tried solving the problem by finding the power values with base 2 and exponent n. It worked for smaller values correctly.
but larger values over 200 such as 255 seems to not give me correct answer, I tried using long long data type but still the answer is wrong.I will try solving this problem and get back to you again.


