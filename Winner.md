## Find the Winner of the Circular Game

### Problem Statement:
There are `n` friends playing a game, sitting in a circle and numbered from 1 to `n` in clockwise order. The rules of the game are as follows:

1. Start at the 1st friend.
2. Count the next `k` friends in the clockwise direction, including the friend you started at. The counting wraps around the circle and may count some friends more than once.
3. The last friend you counted leaves the circle and loses the game.
4. If there is still more than one friend in the circle, go back to step 2, starting from the friend immediately clockwise of the friend who just lost, and repeat.
5. Else, the last friend in the circle wins the game.


### Constraints:

- `1 <= k <= n <= 500`

### Example:

#### Input:
```plaintext
n = 5, k = 2
```
#### Output:
```plaintext
3
```
#### Explanation:
1) Start at friend 1.
2) Count 2 friends clockwise, which are friends 1 and 2.
3) Friend 2 leaves the circle. Next start is friend 3.
4) Count 2 friends clockwise, which are friends 3 and 4.
5) Friend 4 leaves the circle. Next start is friend 5.
6) Count 2 friends clockwise, which are friends 5 and 1.
7) Friend 1 leaves the circle. Next start is friend 3.
8) Count 2 friends clockwise, which are friends 3 and 5.
9) Friend 5 leaves the circle. Only friend 3 is left, so they are the winner.
