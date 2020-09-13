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
