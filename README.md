# -crib_dragging.py
Coursera programming assignment I,Stanford Cryptography I. 

### Problem
#####Many Time Pad 

Let us see what goes wrong when a stream cipher key is used more than once. Below are eleven hex-encoded ciphertexts that are the result of encrypting eleven plaintexts with a stream cipher, all with the same stream cipher key. Your goal is to decrypt the last ciphertext, and submit the secret message within it as solution. 

### crib drag

If cripto 1 and cripto2 has been encrypted using the same stream cipher key so:

cripto 1 XOR cripto2 = (Key XOR  m1)  XOR (Key XOR  m2) = m1 XOR m2

The crib drag attack consist in trying to guess words present in one of the messages (m2 for example) Xor them with the result of (m1 XOR m2) and as result obtain the message m1. Given that if the word is present in m2 the result will be the discovery of part of the message m1 (m2(m2 XOR m1) = m1)

This example uses  one-time pad (OTP) as encryption technique
