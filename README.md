# Elixir List Modification Issue in Enum.each

This repository demonstrates an issue related to modifying a list while iterating over it using `Enum.each` in Elixir.  Because Elixir lists are immutable, attempting to modify the list within the `Enum.each` loop will not produce the expected result. The example shows this behavior and provides a corrected solution.

## Bug
The `bug.ex` file contains the erroneous code that attempts to remove the element `3` from the list during iteration. Although it looks like it should work, it won't because of Elixir's immutability.

## Solution
The `bugSolution.ex` file presents a corrected version using `Enum.filter` to create a new list without the element `3`.