# collatz conjecture implemented using numpy

Unsolved problem in mathematics: Does the Collatz sequence eventually reach 1 for all positive integer initial values? The Collatz conjecture is one of the most famous unsolved problems in mathematics.
The conjecture asks whether repeating two simple arithmetic operations will eventually transform every positive integer into 1.

You'll feel the need. This issue is well stated, understandable, and all too alluring. Simply choose any number: If the number is odd, triple it and add one. If the number is even, divide it in half. Repeat the process with that new number several times. You'll soon find yourself in a loop if you do this. That is, at least, what we anticipate happening.

10 is an even number, therefore we can divide it in half to obtain 5. 5 is odd, so we triple it and add 1.Now that we have 16, which is even, we divide it in half to get 8, then in half again to get 4, then in half again to get 2, and finally in half again to get 1. One is tripled and added because it is strange. We're back at 4, and we already know how this will end: 4 follows 2 and then 1 and then 2 and so on. We've entered a loop.

Try 11 instead: We quadruple it and add 1 since it's strange. Now that we have 34, which is even, we can double that by half to get 17, triple that to get 52, halve that to get 26 to obtain 13, and then triple that and 1 to get 40, halve that to get 20, then 10, then 5, triple that and add 1 to get 16, and halve that to get 8, then 4, 2 and 1. And we’re stuck in the loop again.

According to the controversial Collatz conjecture, if you start with any positive number, you will always wind up in this loop. It appears too easy and organised to resist comprehension. 

It’s easy to verify that the Collatz conjecture is true for any particular number: Just compute the orbit until you arrive at 1. But to see why it’s hard to prove for every number, let’s explore a slightly simpler function,f.

f(n)= {n/2  if n is even 
      {3n+1  if n is odd
 
The functionℊ is similar to f, but for odd numbers it just adds 1 instead of tripling them first. Since ℊ and f are different functions, numbers have different orbits under ℊ than under f. For example, here are the orbits of 10 and 11 under f:

10 → 5 → 6 → 3 → 4 → 2 → 1 → 2 → 1 → 2 → ...
11 → 12 → 6 → 3 → 4 → 2 → 1 → 2 → 1→ 2 → ...
