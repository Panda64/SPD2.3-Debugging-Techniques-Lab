# Debug Log

**Explain how you used the the techniques covered (Trace Forward, Trace Backward, Divide & Conquer) to uncover the bugs in each exercise. Be specific!**

In your explanations, you may want to answer:

- What is the expected vs. actual output?
- If there is a stack trace, what useful information does it contain?
- Which technique did you use, on which line numbers?
- What assumptions did you have about each line of code, and which ones were proven to be wrong?

_Example: I noticed that the program should show pizza orders once a new order is made, and that it wasn't showing any. So, I used the trace forward technique starting on line 13. I discovered the bug on line 27 was caused by a typo of 'pzza' instead of 'pizza'._

_Then I noticed another bug ..._

## Exercise 1

- Added `backref` to `toppings` in `Pizza` class in order to properly connect the two classes.
- Changed the from names in the `/order` route to properly reflect the names in `order.html`
- Fixed a typo in the topping for loop (located in the `/order` route) to properly allow toppings to get appended to the `Pizza` object.
- Added a database commit at the end of the `/order` route to properly save the order to the database.
- Changed redirect url in `/order` route to properly redirect back home.

Almost all of these errors were discovered by going along and fixing one error after the other.

## Exercise 2

- Changed variables in `/results` route to properly reflect the names in `results.html`
- Changed API url to `https` instead of `http`
- Changed url parameter name to reflect API docs
- Changed result query names to reflect API docs

All of these bugs and errors were discovered with the help of turning debugging on in `app.run()`.

## Exercise 3

Merge Sort:

- Returned `arr` in base case
- Fixed index mismatch in one of the while loops that check if any elements were left.
- Incremented k in each of the while loops to put selected elements in the proper place.

Binary Search:

- Used floor division to calculate the midpoint in order to avoid float values.
- Changed how `low` and `high` were calculated.
- Incremented and decremented `mid` in respective `if` statements.
