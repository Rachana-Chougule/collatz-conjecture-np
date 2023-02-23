# collatz conjecture implemented using numpy

Unsolved problem in mathematics: Does the Collatz sequence eventually reach 1 for all positive integer initial values? The Collatz conjecture is one of the most famous unsolved problems in mathematics.

The conjecture asks whether repeating two simple arithmetic operations will eventually transform every positive integer into 1.
You'll want to. This issue is well-stated, easy to comprehend, and alluring. Select any number you want: Triple the number and add one if it is odd. Divide the number in half if it is even. With that new number, carry out the procedure several times. If you do this, you'll soon be stuck in a loop. At the very least, that is what we anticipate taking place.

Given that 10 is an even number, we can divide it in half to get 5. 5 is odd, so we triple it and add 1. When we have 16 (which is even), we divide it in half to get 8, then in half to get 4, then in half to get 2, and finally in half to get 1. Due to its strangeness, one is tripled and augmented. We are back at 4 now, and the way this will end is already known: 4 comes after 2, followed by 1, and so on. We are now in a loop.

Instead, try 11: Because it's odd, we quadruple it and add one. Now that we have 34, which is equal, we can double it by half to get 17, triple it to get 52, halve it to get 26 to get 13, triple it to get 40, halve it to get 20, 10, 5, triple it to get 16, and halve it to get 8, 4, 2, and 1. Additionally, we have relapsed into the loop.

The controversial Collatz conjecture states that this loop will always begin with any positive number. It appears to be organized and simple enough to comprehend. 

It is simple to demonstrate that the Collatz conjecture holds true for any number: Simply calculate the orbit until you reach 1. But let's look at a slightly simpler function, f, to see why it's hard to prove for every number.
It’s easy to verify that the Collatz conjecture is true for any particular number: Just compute the orbit until you arrive at 1. But to see why it’s hard to prove for every number, let’s explore a slightly simpler function,f.

f(n)= {n/2  if n is even 
      {3n+1  if n is odd
 
The functionℊ is similar to f, but for odd numbers it just adds 1 instead of tripling them first. Since ℊ and f are different functions, numbers have different orbits under ℊ than under f. For example, here are the orbits of 10 and 11 under f:

10 → 5 → 6 → 3 → 4 → 2 → 1 → 2 → 1 → 2 → ...

11 → 12 → 6 → 3 → 4 → 2 → 1 → 2 → 1→ 2 → ...
