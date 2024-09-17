# OVERVIEW
Algorithms are essentially methods, but some are more efficient than others
Efficiency refers to the amount of work for the processor, memory used, I/O costs

# HOW TO COMPARE
Consider washing dishes:
We have a stack of n dishes to wash and dry by hand.
1. Prepare sink (5 minutes)
- Cannot avoid, every step must involve this
2. Wash and rinse each dish (0.5 minutes each)
3. Dry each dish (0.5 each)

This creates a growth function, takes an input and outputs how much work
will be done

f(n) = 5 + 0.5n + 0.5n
or f(n) = 5 + n

Careless way
1. Again, prepare sink (5 minutes)
2. Wash and rinse each dish the same time (0.5 minutes), but water goes everywhere
3. Dry (and redry) each washed dish

f(n) = 5 + 0.5n + Summation * 0.5

Now comparing...
First way, take 10 dishes + 5 = 15
But with the careless way, 10 dishes + 3/4n + 1/n^2 = 37.5

The two solutions are both correct, but the first way is obviously more efficient.

# Order of the Algorithm
The dominant factor, as n becomes large is the order (or Big-O notion)
As the algrotihm function becomes larger, where is the worst case scenario?

For the careful wash, the notion is O(n), where the dishes being washed is the
worse.
For the careless wash, the notion is O(n^2) where the dishes are being re-dried is the worse category since it is quadratic

Germ-o-phobe way:
What is the growth function, the order, and compare to the others?
Clean and prepare sink before each dish (10 mins)
Wash each dish (0.5 second)
Dry each dish (0.5 second)

f(n) = 10n + 0.5n + 0.5n = 11n
is the growth function

The order is O(n), the coefficient can be disregarded

This method is still better than the careless wash, since it is linear.

# Common Orders for single variable algorithms
Some algorithms operate as constant time methods O(n^0) = 1, such as the length() method, when evaluating size of arrays.

Logarithmic functions utilize a stair step method to represent, where each stair step is twice as long as the value before it. Not very common O(log n)

Similarly log-linear has a value n, that multiplies the log value O(n log n)

Linear algorithms are generally characterized by a single loop. toString() is an example on a collection. O(n)

A quadratic algorithm is often a nested loop, concatenation (string addition) is an example. O(n^2)

Three nested loops is a cubic algorithm. O(n^3)

Exponential algorithms, not to be confused with quadratic, this is the basis of
encryption. 258 bit encryption is viewed as O(n^258)