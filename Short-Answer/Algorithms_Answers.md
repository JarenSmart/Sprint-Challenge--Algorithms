#### Please add your answers to the **_Analysis of Algorithms_** exercises here.

## Exercise I

a)

<!-- ```python
a)  a = 0
    while (a < n * n * n):
      a = a + n * n
``` -->

This is an example of constant time because the value 'a' is not dependent on the size of 'n'.

b)

<!-- ```
b)  sum = 0
    for i in range(n):
      j = 1
      while j < n:
        j *= 2
        sum += 1
``` -->

This is an example of O(n^2) due to the number of inner(nested) loops we perform on 'n'.

c)

<!-- ```
c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)
``` -->

This is an example if linear or O(n) time due to the variable bunnies being decremented by a constant amount.

## Exercise II

<!-- Suppose that you have an n-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor f or higher, and doesn't get broken if dropped off a floor less than floor f. Devise a strategy to determine the value of f such that the number of dropped + broken eggs is minimized.

Write out your proposed algorithm in plain English or pseudocode AND give the runtime complexity of your solution. -->

- The start of the building can be an array of sorted floors. Lowest floor number being the beginning of the array up to the final and highest floor.
- To begin the testing of egg breakage or not, we could cut the floors in half and test the middle most floor and see if an egg breaks.

  1. If the egg breaks, we know that it will continue to break at higher heights.Therefore, eliminating the need of testing higher floors.
  2. If the egg doesn't break, we continue climbing the floors until it does break. Leaving you with the answer of which floor was the last to leave the egg unbroken and which floor it finally broke on.

- I think this approach is log(n) at best due to the testing that would be necessary to find the given answer while clearly giving you a result of each floor.
