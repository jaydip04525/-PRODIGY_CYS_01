# Caesar Cipher Encryptor and Decryptor
This Python code implements a Caesar Cipher, which is a simple encryption technique. It works by shifting each letter in a message by a certain number of positions down the alphabet.
# The Code Breakdown:
The code is divided into three functions:
1. encrypt(message, key) : This function takes a message and a key as input. It iterates over each character in the message and checks if it's an alphabetical character (a-z, A-Z).

🔘If it is alphabetical, it performs the shift based on the key value.


  ◽It converts the character to its corresponding ASCII code.
  
  ◽It adds the key value to the ASCII code.
  
  ◽It takes the modulo 26 of the sum to handle overflow (resulting in a value between 0-25).
  
  ◽It converts the new ASCII code back to a character.

  
🔘If the character is not alphabetical, it remains unchanged.

2. decrypt(encrypted_message, key): This function works similarly to the encryption function, but it subtracts the key value from the ASCII code to shift the letters back to their original positions.

3. main(): This function is the entry point of the program. It prompts the user for a message and a key, encrypts the message using the encrypt function, decrypts the encrypted message using the decrypt function, and then prints both the original and encrypted messages.
# Limitations:
This is a basic Caesar Cipher and has limitations:

🔘It only encrypts alphabetical characters (a-z, A-Z).

🔘It's not a secure encryption method, as someone can easily crack the code by trying different key values (brute-force attack).
