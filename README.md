# RSA-and-Digital-signature-Project

## Overview
Implemented RSA encryption and applied it to digital signature. This project was divided into two parts: 1) RSA key generation and
2) Generate and verify digital signatures using a SHA-256 hash.

## Key Steps
**Part 1: RSA key generation.**
  - Implement Fermat test.
  - Use Fermat's test to generate two large prime numbers (p,q), each should have a size between 128 and 256 bits.
  - Save p and q in a file named p_q.txt, one integer per line and make sure no white space saved.
  - Use the extended Euclidean algorithm to generate two pairs of keys: (e,n), (d,n), where n = p * q.
  - Save the two pairs of keys in two separate files: e_n.txt and d_n.txt, one integer per line and no white space.

**Part 2: Generate and verify digital signatures using a SHA-256 hash.**
  - **Sign a given file**
    - Generate a SHA-256 hash of the content of the file to be signed.
    - Sign/"decrypt" this hash value using the private key stored in d_n.txt.
    - Combine the original content and the signature into one document.
    - Append the 64-byte signature at the end of the original content.
  - **Verify the signed file**
    - Separate the signature from the content of the file in the signed document.
    - Generate a SHA-256 hash of the content of the file you have signed.
    - Check if the signature (old hashcode/m) = new SHA-256 hashcode/m.

## How to Run
1. Clone this repository:
```bash
git clone https://github.com/BLynch16/RSA-and-Digital-signature-Project.git
cd RSA-and-Digital-signature-Project
```

3. Launch Jupyter:
```bash
jupyter notebook
```

4. Open 'Algorithms_Project1.ipynb' and run the cells in order.


