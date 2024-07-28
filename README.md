# Miscellaneous lists of primes

## Pseudo-Mersenne primes

```psmersenne.csv``` and ```psmersenne.txt```

List of ```2**N -C``` primes, with the smallest suitable ```C```.
Complementing the smallest such ```C``` value for each ```N``` bitcount,
we also list the smallest suitable prime of form ```4k+1``` or
```4k+3``` (for ```...-C``` 3 mod 4, or 1 mod 4, respectively), such as
for cases where modular square root computation needs to be efficient
[S24, section 2].

In addition to primes of the form ```2**N -C```, we list the smallest
```2**N +E```. Allowing similarly efficient implementation, the order of
these finite fields allows processing ```N```-bit inputs.

Fields of ```.csv```:

1.  ```N```
2.  ```C``` of largest ```2**N -C``` prime
3.  ```C``` in hex
4.  ```D``` of ```2**N -D``` prime with ```3 mod 4```, if ...```-C``` is
    ```1 mod 4```
5.  preceding field, in hex, if present
6.  ```D``` of ```2**N -D``` prime with ```1 mod 4```, if ...```-C``` is
    ```3 mod 4```
7.  preceding field, in hex, if present
8.  ```E``` of smallest ```2**N +E``` prime
9.  ```E``` in hex
10. ```F``` of ```2**N +F``` prime with ```3 mod 4```, if ...```+E``` is
    ```1 mod 4```
11. preceding field, in hex, if present
12. ```F``` of ```2**N +F``` prime with ```1 mod 4```, if ...```+E``` is
    ```3 mod 4```
13. preceding field, in hex, if present

Hex fields are obviously redundant, included only for readability. The
```.txt``` version is simply monospace-formatted from ```.csv```.


# References

[S24]
Scott: Elliptic Curve Cryptography for the masses: Simple and fast
finite field arithmetic
  eprint.iacr.org/2024/779
  version of 2024-06-24  [accessed 2024-07-28]
  SHA-256(PDF)=
    0171a48e74cfdd218fc0eb536d20934020180dffd242ce6c69fa2ccea6a66897

