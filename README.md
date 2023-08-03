# Takeaway Game - Code Challenge

## Description

The "takeaway" game is played by two players using a number of stones. The first player goes first and can take 2, 3, or 5 stones from the pool. The second player goes next and can also remove 2, 3, or 5 stones. The players take turns until there are fewer than 2 stones left, and the player unable to move loses.

This challenge requires you to write a function that determines whether the active player can win a game with a given number of stones, assuming both players play perfectly (i.e., they always make the best possible move).

## Function Signature

```javascript
function canWin(n) {
  // Implementation goes here
}
```

## Input

- `n` (integer): The initial number of stones in the game.

## Output

- Returns `true` if the active player can win the game starting with the given number of stones, and `false` if not.

## Examples

```javascript
canWin(1);   // false
canWin(2);   // true
canWin(3);   // true
canWin(4);   // true
canWin(5);   // true
canWin(6);   // true
canWin(7);   // false
canWin(8);   // false
canWin(9);   // true
canWin(10);  // true
```

## Implementation

The provided function `canWin` uses recursion and memoization to calculate the result. It follows a recursive approach to check all possible moves from the current number of stones (2, 3, and 5) and stores the results in a memoization table to avoid redundant calculations and improve performance. The memoization ensures that we only compute the result for each number of stones once.

The function is implemented in JavaScript, and it returns `true` if the active player can win the game and `false` otherwise.

Feel free to use this function to determine the winning strategy in the "takeaway" game with different numbers of stones. Enjoy the challenge!