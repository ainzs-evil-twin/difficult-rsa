# difficult-rsa

An RSA challenge from Ainz's evil twin.

**Note:** Even though n is small, use logical thinking and avoid brute-force

## Description

Alice and Bob are best friends. To show the depth of their friendship, **they decide to use the same p** for their RSA public keys.  
We managed to get our hands on their public keys, [alice.txt](../main/alice.txt) and [bob.txt](../main/bob.txt)  
We were also able to intercept a message sent from Alice to Carol. It said:
`4188713224811729923338308470142557182203691002856253245778138032264225662538339973035444057293733531104457410423739321918076207587152546291602684395254731`  
Can you decrypt this ciphertext with given hints?

## Attachments

`https://github.com/ainzs-evil-twin/difficult-rsa/blob/main/alice.txt`  
`https://github.com/ainzs-evil-twin/difficult-rsa/blob/main/bob.txt`

## Flag format

`ictf{.+}`

## Category

Crypto

## Hints

<details> 
    <summary>Hint 1</summary> 
    How could using same p make n vulnerable for both of them?
</details>