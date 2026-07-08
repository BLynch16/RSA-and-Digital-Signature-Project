# RSA-and-Digital-signature-Project

## Overview
Implemented RSA encryption and applied it to digital signature. This project was divided into two parts: 1) RSA key generation and
2) generate and verify digital signatures using a SHA-256 hash.

## Key Steps
**Part 1: RSA key generation.**
  - Implement Fermat test.
  - Use Fermat's test to generate two large prime numbers (p,q), each should have a size between 128 and 256 bits.
  - Save p and q in a file named p_q.txt, one integer per line and make sure no white space saved.
  - Use the extended Euclidean algorithm to generate two pairs of keys: (e,n), (d,n), where n = p * q.
  - Save the two pairs of keys in two separate files: e_n.txt and d_n.txt, one integer per line and no white space.
