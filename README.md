# Affine-encryption

1. First we give a list of lowercase alphabets and a list of uppercase alphabets.

2. We go through the whole alphabet and we add the lowercase alphabet and the uppercase alphabet to each run.

3. We create a function that returns the gcd of two numbers a and b, that changes the position of a and b at each run and performs the modulo of a and b.

4. Then we have an Affine encryption function which takes a, b and L as parameters which will be used later for the encryption of our message, at the start we will test if the letter is uppercase or lowercase, then we will look for the index of the letter qu 'we will use by applying the formula Y=(ax+b) mod 26 where y is the index of the number letter otherwise if the letter is not in the alphabet we (symbol) we will return it.

5. Then we have two functions to calculate the inverse of a number a, the 1st was not seen in progress but it requires fewer operations than the one seen in progress and for that we took it but c does not change not much since the complexity remains the same for both algorithms. For the 1st function it will take as parameter a will give its modular inverse 26 of a number for that we initialize x to 0 and we use a loop as long as a*x%26 is not different from 1, x takes the value of x + 1 and ends up returning the value of x at the end. And for the 2nd function of Euclid we apply exactly the formula seen in progress for the extended Euclid algorithm

6. Thereafter we have a decryptionAfiine function which takes the same parameters of the encryptionAffine function and which does the same thing as the encryptionAffine function but the only difference is that y takes the value of (the inverse of a)*(x-b) modulo 26. Initially we will test if the letter is an uppercase or lowercase letter after we retrieve the index of the letter that we will use to find the index of the deciphered letter using the formula mentioned above otherwise if the letter is a symbol we'll send her back.

7. We have two functions, one crypt and the other decrypt, one which is used to encrypt our Test sets using the encryptionAffine function and the other is used to decrypt our message, using the decryptionAffine function they will both call the encryptionAffine and decryptionAffine functions n times with n equal to the size of the message.

8. Finally, the encrypted messages and the decrypted messages are displayed.
