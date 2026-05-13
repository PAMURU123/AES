# EX-8-ADVANCED-ENCRYPTION-STANDARD ALGORITHM
## Name:PAMURU VENKATESH
## Reg. no:212224040230
# Aim:
To use Advanced Encryption Standard (AES) Algorithm for a practical application like URL Encryption.

# ALGORITHM:
1. AES is based on a design principle known as a substitution–permutation.

2. AES does not use a Feistel network like DES, it uses variant of Rijndael.

3. It has a fixed block size of 128 bits, and a key size of 128, 192, or 256 bits.

4. AES operates on a 4 × 4 column-major order array of bytes, termed the state

# PROGRAM:
```
#include <stdio.h> 
#include <string.h> 
void xorCrypt(char *in, char *key) { 
for (int i = 0; in[i]; i++) in[i] ^= key[i % strlen(key)]; 
} 
int main() { 
char msg[] = "VENKY", key[] = "secretkey"; 
printf("Original: %s\n", msg); 
xorCrypt(msg, key); 
printf("Encrypted: %s\n", msg); 
xorCrypt(msg, key); 
printf("Decrypted: %s\n", msg); 
return 0; 
} 


```


# OUTPUT:
<img width="1679" height="801" alt="image" src="https://github.com/user-attachments/assets/efb931da-0e88-4dd3-8b4f-3ddd1c2816bc" />


# RESULT:


The program is executed successfully.



