# Python notes



## 1.   **[Hint].** If you're getting a `local variable [var] reference before assignment` error:

This happens because in Python, you aren't normally allowed to modify variables defined in parent frames. Instead of reassigning `[var]`, the interpreter thinks you're trying to define a new variable within the current frame. We'll learn about how to work around this in a future lecture, but it is not required for this problem.

To fix this, you have two options:

1) Rather than reassigning `[var]` to its new value, create a new variable to hold that new value. Use that new variable in future calculations.

2) For this problem specifically, avoid this issue entirely by not using assignment statements at all. Instead, pass new values in as arguments to a call to `announce_highest`.

