# BCrypt

## Hashing
[Notes taken from this site](https://auth0.com/blog/hashing-passwords-one-way-road-to-security/)

- Credentials need to be stored on the server side to provide a comparison.
- A simple method is to store them in a table that maps a username to a password.
- The most basic, and least secure, method is a storage format called *cleartext*
- *plaintext* != *plain text*
- *plain text* = unformatted text.
- *plaintext* = data input to a cryptographic algorithm.
- *Hashing* = transforming passwords so they can't be converted back to their original form.
- >In cryptography, a hash function is a mathematical algorithm that maps data of any size to a bit string of a fixed size.
- *avalanche effect* = if an input is changed slightly, the output is changed significantly.
- Hash functions are deterministic, which means the same input will always result in the same output.
- *Rainbow table attack* = an attacker can use a large database of precomputed hash chains to find the input of stolen password hashes.
- >Since a rainbow table attack has to re-compute many of these operations, we can mitigate a rainbow table attack by boosting hashing with a procedure that adds unique random data to each input at the moment they are stored. This practice is known as **adding salt to a hash** and it produces **salted password hashes**.

## BCrypt
[Notes taken from this site](https://danboterhoven.medium.com/why-you-should-use-bcrypt-to-hash-passwords-af330100b861)

- >Using a Key Factor, BCrypt is able to adjust the cost of hashing. With Key Factor changes, the hash output can be influenced. In this way, BCrypt remains extremely resistant to hacks, especially a type of password cracking called rainbow table.

[Back to HOME](../README.md)