# Find value of x

## Problem Analysis
- As for r 2^50 values are possible and only one transcript is available
- Hashing has no role in the security of exrtracting the value of r
- phi(p) = p - 1
- Schnorr security completely collapses if the nonce r is small or biased; even a 50-bit nonce allows recovery of the secret x via algebraic attacks

We will use pollards kangaroo algorithm for this case because : 
- Schnorr security assumes uniform random nonces
- Pollard Kangaroo is designed for this exact situation
- Hashing the challenge does nothing to fix bad randomness

## Value of x

```python
x = 
```
