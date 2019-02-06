# cryptography

This project creates a secured connection between client and the server. 
Wherein we have already hard coded the hostname and port number in the client 
and server programs to avoid any port number error causing 
overrides on the current ongoing ports of the computer. 

## Part A

We have created RSA class and it can run independently as well as along with complete code. 
It was written so as to test the modules separately. 
This RSA class uses BigInteger and Random inbuilt classes of java in order to calculate the two largest prime numbers. 

### Executing the code

```sh
$ java RSA
```
Then enter the desired message.

## Part B

We have created OneTimePadCipher class and it can also run independently as well as along with complete code. 
It was written so as to test the modules separately. 
This class performs the basic operations of xor and binary and decimal conversions.

### Executing the code

```sh
$ java OneTimePadCipher
```
Then enter the desired message.

## Part C

We have created two different classes one for Client and one for Server. 
Wherein we have integrated the RSA and OneTimePadCipher classes in the client and server program in order to secure the transmission. 
The encryption is taking place at the client end using public and private keys from RSA class and being sent to the server. 
The server then reads the encrypted message and decrypts the message using the keys. 
These keys are exchanged internally through the RSA class itself to provide security for the keys as well.

### Executing the code

Open 2 terminals.

In first write

```sh
$ java Server
```

In second write

```sh
$ java Client
```
Then enter the desired message.
