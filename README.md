## Number of Provinces

###Problem Statement:
There are `n` cities. Some of them are connected, while some are not. If city `a` is connected directly with city `b`, and city `b` is connected directly with city `c`, then city `a` is connected indirectly with city `c`.

A **province** is a group of directly or indirectly connected cities and no other cities outside of the group.

You are given an `n x n` matrix `isConnected` where `isConnected[i][j] = 1` if the `i-th` city and the `j-th` city are directly connected, and `isConnected[i][j] = 0` otherwise.

### Constraints:
- `1 <= n <= 200`
- `n == isConnected.length`
- `n == isConnected[i].length`
- `isConnected[i][j]` is either `1` or `0`.
- `isConnected[i][i] == 1` (a city is always connected to itself)
- `isConnected[i][j] == isConnected[j][i]` (connections are bidirectional)

### Example:
![](provinces.jpg)
#### Input:
```plaintext
isConnected = [[1,1,0], 
               [1,1,0], 
               [0,0,1]]
```
#### Output:
```plaintext
2
```
