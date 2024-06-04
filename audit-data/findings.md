### [S-N] Storing the password on-chain makes it visible to anyone and no longer private 

**Description:** All data stored on-chain is visible to anyone and can be read directly from the blockchain. The `Password::s_password` variable is intended to be a private variable and only accesed through the `Password::getPassword` function, which is intended to be only called by the owner.

We show one of reading such data on-chain below

**Impact:** Anyone can read the private password severly breaking the functionality of the protocol

**Proof Of Concept:** (Proof of Code) 

The below test case shows that anyone can read the password directly from the blockchain

**Recommended Mitigation:**