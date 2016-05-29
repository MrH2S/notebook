## comprehension
example1:
```haskell
[2*n | n <- [2,4,7]]
```
so, the list is transformed by another list.

- the left of '|' is transform function generate the target list from source list
- the right of '|' is source list elements generator

example2 with test:
```haskell
[2*n | n <- [2,4,7], isEven n, n > 3]

[m + n | (m,n) <- [(2,3),(2,1),(7,8)], m<n]
```
- can only test by Bool Type
