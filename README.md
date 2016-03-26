# Prime-Sive
DESCRIPTION

It begins with the only true prime pair 2 and 3, whose product forms the magical composite number 6. 
All other primes orbit around it and its multiples. Using alternating patterns of 2 and 4, 
the composites are revealed in succession beginning with 5 in the first segregated pair of the series. 
Each integer in the series is raised to the second power and then its product of 2 and 4 reveals the distribution of the composite numbers.
As the process is repeated, the order that 2 and 4 are used to generate the products alternates, 
to progressively strip away the remaining composites integers and reveal the rest of the primes. 

The segregated pairsList
Other than 2 and 3 all prime numbers are located adjasent to a multiple of 6, this maens we can ignore other intergers in our seach for primes.

The following expression can be used and repeated to generate the segregated pairsList of multiples of 6-1 and 6+1.
Begining with a = 5 
a² + (a x 2) = b² - (b x 2)
b² + (b x 4) = c² – (c x 4)
c² + (c x 2) = d² - (d x 2)
d² + (d x 4) = e² – (e x 4)...........

When setting a maxValue of 100, this generates the following segregated pairsList:-
[5, 7, 11, 13, 17, 19, 23, 25, 29, 31, 35, 37, 41, 43, 47, 49, 53, 55, 59, 61, 65, 67, 71, 73, 77, 79, 83, 85, 89, 91, 95, 97...]

Revaling the composites in the pairsList
While threre is no patern to the distribution of the primes, there is a patern to the composite numbers in the list, all of the segregated pairs in the series are primes up untill a². The composites in the segregated pairsList are revealed in a two step alternating pattern.

STEP ONE
a² is the first composite in the list. from a² onwards further composites (all multiples of a) occur with the following regularity:-
a = 5  (the first integer the pairsList)
a² = first composite
a² + (a x 2) = second composite
second composite + (a x 4)
this process gets repeated by adding the alternating products of a x 2 then a x 4 to the previous composite.

This reveals the composite products of a, in the segregated pairsList:-
[25, 35, 55, 65, 85, 95...]

STEP TWO
Similar to step one only here the polarity of 2 and 4 is reversed
b = 7 (the second integer the pairsList)
b² = first composite
b² + (b x 4) = second composite
second composite + (b x 2)
this process gets repeated by adding the alternating products of b x 4 then a x 2 to the previous composite.

This reveals the composite products of b, in the segregated pairsList:-
[49, 77, 91...]

Steps one and two are repeated sequentialy creating loopListOne and loopListTwo throghout the pairsList untill n² > maxValue, loopListOne and loopListTwo are combined forming a compositeList and the compositeList is striped from the pairsList to form the primesList. Lastly the prime pair 2 and 3 are added to the primesList.



