# not-so-difficult-rsa

An RSA challenge from Ainz's evil twin.

**Note:** Even though n is small, use logical thinking and avoid brute-force

## Description

Alice and Bob are best friends. To show the depth of their friendship, **they decide to use the same p** for their RSA public keys.  
We managed to get our hands on their public keys, [alice.txt](../main/alice.txt) and [bob.txt](../main/bob.txt)  
We were also able to intercept a message sent tp Alice from Carol. It said:
`4188713224811729923338308470142557182203691002856253245778138032264225662538339973035444057293733531104457410423739321918076207587152546291602684395254731`  
Can you decrypt this ciphertext with given hints?

## Attachments

`https://github.com/ainzs-evil-twin/not-so-difficult-rsa/blob/main/alice.txt`  
`https://github.com/ainzs-evil-twin/not-so-difficult-rsa/blob/main/bob.txt`

## Flag format

`ictf{.+}`

## Category

Crypto

## Hints

<details> 
    <summary>Hint 1</summary> 
    Is there to find a number p which divides two given numbers n1 and n2?
</details>
<details> 
    <summary>Hint 2</summary> 
    You have to use the n from alice.txt to get final answer.
</details>
<details> 
    <summary>Hint 3</summary> 
    Computers don't work on decimal numbers, resulting in some strange behaviour when dealing with very large decimals.  
	I suggest you to use any tool or library specifically built for working with RSA only you have obatained p. If you are writing the algorithm yourself, be mindful of division of large numbers and modular arithmetic. For example in python, I suggest you to use `decimal` module and set `getcontext().prec` to a high value like 250. Not doing so may result in you getting garbage value even if your p is correct
</details>
