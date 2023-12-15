Shors algorithm is a quantum algorithm used to find the factors of a number, specifically the prime factors of a number which can be factorized into exactly two prime factors.
It converts the factor finding problem into a period finding problem.
Choose a number a which is coprime to the number N whose factors we want to find. In this program, we are finding the factors of 15 and we choose a as 2.
Now find the period of the function f(r)=(a^r)%15. In this case it is actually 4. 
Now the factors are gcd(r+1,15) or gcd(r-1,15). If we obtain one factor as n1, the other factor can be found by 15/n1.
If the factors generated are equal to 1, discard it and try again as 1 is not a prime factor.
