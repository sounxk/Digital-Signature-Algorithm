# Digital-Signature-Algorithm

Electronic digital signature for text files. Needed for Labs on Information Theory, 4 labs. Implemented on the basis of the SHA-1 hash function, according to the DSS standard.

### Theory
--------------------------------------------------------------------------------------------------------------------------------------

***The Digital Signature Algorithm (DSA) is a digital information technology that has been developed for the digital signatures and the discrete logarithm problem.***

***Signing***
* Generate a random per-message value k where 1<k<q;
* Calculate r = (g**k mod p) mod q;
* Calculate s = k**-1(Hash(m)+x*r) mod  q;
* In the unlikely case that r=0 or s=0, start again with a different random k;
* The signature is (r,s).
