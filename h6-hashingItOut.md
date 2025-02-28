# One-way functions (x)
> Summary of:
> Applied cryptography: chapter 2.3 - One-way functions (Schneier, 2015)

One way function
- One way functions are easy to compute, but infeasible to reverse


One way-hash function
- The mechanics of a one-way hash function is pretty straight forward
  - Take a variable size string (pre-image) --> run it through the mathematical function --> out comes a fixed-length string (hash value)
- The key thing here, is that it's easy to calculate the hash value from the pre-image,
but it's hard to get a pre-image to match a certain hash value.
- A good one-way hash function is also collision free: meaning it's extremely challenging to produce 2 pre-images with the same hash value.


