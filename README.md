# Consecutive-non-prime-with-Rabin-Miller-Algorithm

This program answers the question as follows:
Given a positive integer n, what is the first appearance of n consecutive non primes?

The original question is as such: Can there be 2000 consecutive non-prime numbers?

The answer is yes, for any given number n, an obviously true example is (n+1)! + 2 to (n+1)! + n + 1. This answer however is obviously not the smallest. For example, for n = 3, the answer is 25 to 27, however the smallest is 8 to 10.

This is actually called a prime gap: https://en.wikipedia.org/wiki/Prime_gap. People have extensively calculated this. Calculating 2000 consecutive non-prime numbers is equivalent to calculating a prime gap >= 2001

With my python program it is very easy to confirm cases for n <= 150. But when n increases to 200, runnning time becomes 6 min.

Indeed to calculated large prime gap isn't such an easy task.

However using the Rabin Miller Algorithm: http://inventwithpython.com/cracking/chapter22.html, we can very quickly confirm if a very large number is a prime number.

Using the results that other people have already calculated, we can confirm if the prime gap actually exist: https://faculty.lynchburg.edu/~nicely/gaps/g2k.html

The results confirms that the first appearance of 2000 non-prime numbers are: the 2000 numbers after 2681804411030606193859004129 (28 digits), prime gap is 2030.

The first appearance of just 2000 consecutive non-prim numbers ( prime gap = 2002 ) are: the 2000 numbers after 824742086414264032043746981329337.
