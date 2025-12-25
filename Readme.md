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

```sh
# run to run the attack
sage attack.sage

# To verify the attack run
sage check.sage
```

```python
x = 129741816436586536192511069033522723797805991085207391260653840826086090109
```
