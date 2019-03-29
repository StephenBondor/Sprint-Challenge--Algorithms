Add your answers to the Algorithms exercises here.

I.a)

The runtime complexity is O(n^3) because for the input size of (n) the program
must run n x n x n loops on that input.

I.b)

The runtime complexity is O(n^3) because for each input size (n) the program
must run 3 nested loops iterating over (n). Their are four nested loops, but the
last loop has a constant run time of (k): the range k+1 to k+10 is always 10.
Consequently this converts O(kn^3) to O(n^3)

I.c)

The runtime complexity is either O(bunnies) because for each call of bunnyEars()
it calls the number of (bunnies) recursively. this translates to O(n). Or it is
O(0) because the question asks for runtime complexity of (n) and (n) is never
used in this function. Can't have a run time complexity in (n) if (n) doesn't
exist.

II.

1. I would throw an egg off the first floor, it would break, thus, _f_ is 0.

The runtime complexity of this is O(1)

Obviously this is not the spirit of this question. Thus, To solve for _f_, I
would implement a divide on conquer strategy--similar to binary search.

1. If the heigh of the building is known, find the height of the building.
2. Either divide the height of the building in half or choose a random variable
   between 0 and 200 (the assumed upper limit of floors presently possible to
   construct).
3. I would throw an egg off of that floor.
4. If the egg breaks, I would divide that floor number by 2 and subtract it from
   the current floor. If it does not break, I would divide that floor number by
   2 and add it to the current floor.
5. I would then repeat the test (goto: step 3) until I was at the egg breaking
   threshold, which would give me _f_

The runtime complexity of the second answer is O(log(n)) as this is the runtime
complexity of a binary search tree, which is the method I have implemented.
