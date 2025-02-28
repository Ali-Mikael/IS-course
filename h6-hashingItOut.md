# Applied cryptographty (x)
> Applied Cryptography: Protocols, Algorithms and Source Code in C, 20th Anniversary Edition - Bruce Schneier

**Chapter 2.3 / One-way function**
- One way functions are easy to compute, but infeasible to reverse.
- They play a central role in public-key cryptography, as the functions are extremely challenging to reverse, without the private-key.
- The afore mentioned method is called a *trapdoor one-way function*
  - The public-key (one-way function) is used to encrypt the data, and can only be decrypted using a corresponding private-key (the secret trapdoor).

  
**Chapter 2.4 / One way-hash function**
- The mechanics of a one-way hash function is pretty straight forward
  - Take a variable size string (pre-image) --> run it through the mathematical function --> out comes a fixed-length string (hash value)
- The key thing here, is that it's easy to calculate the hash value from the pre-image,
but it's hard to get a pre-image to match a certain hash value.
- A good one-way hash function is also collision free: meaning it's extremely challenging to produce 2 pre-images with the same hash value.


