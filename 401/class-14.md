# BCrypt

### Intro to Password Hashing
- Storing passwords is risky and complex
- What's hashing?
  - hashing refers to 'chopping something into small pieces'
  - a hash function is a mathematical algorithm that maps data of any size to a bit string of a fixed size. We can refer to the input as the **message** and the output as the **hash** or **message digest**
  - It's easy to compute the hash, but difficult if not impossible to re-generate the original input if only the hash(output) is known
  - It's difficult to creaet an initial input that would match a specific desired output.
  - In contrast to encryption, hashing is a one-way mechanism. The data that is hashed cannot be practically "unhashed"
  - Cryptographic Hash Functions are practically irreversible
    - This is done by using mathematical operations that are extremely difficult to revert like the modulo operator, The original operands are untracable given the result of the operation.
  - A small change in the input has a big impact in the output
  - Hash functions are very useful for securing passwords because they are deterministic
    - a deterministic function is a function that always returns the same output given the same input
  - Limitations of Hash Functions:
    - if a lot of users have the same password, they will share the same hash.
    - salting hashes: adding unique random data to each input at the moment they are stored.
  - To be a cryptographic hash function: a hash function must be pre-image and collision resistant
  - Password hashing is used to verify the integrity of your password, sent during login against the stored hash so that your actual password is never stored.

### bcrypt overview
  - bcrtpy uses a key factor to adjust the cost of hashing. With key factor changes, the hash output can be influenced. This ultimately slows down the cracking process until it's no longer a viable strategy.

