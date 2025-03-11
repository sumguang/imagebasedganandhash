# imagebasedganandhash


Title ： Secure Image Encryption Using Pseudorandom Number Generator based on LSGAN and Hash


Deep learning has been extensively applied in image-related tasks, and recently, Generative Adversarial Networks (GANs) have been utilized to train pseudorandom number generators (PRNGs) for generating pseudorandom sequences. These sequences are used in stream cipher-based image encryption systems. In the context of image encryption, the key is a critical component that must meet specific criteria, such as randomness, sufficient key space, and uniqueness. However, existing approaches often fall short of fulfilling these requirements effectively. This paper introduces a novel PRNG based on Least Squares Generative Adversarial Networks (LSGAN), which is combined with hash functions and neural networks. Building upon this PRNG, an image encryption scheme is proposed. In this scheme, both the sender and receiver share a compact, randomly generated key. This short key is fed into the LSGAN-based PRNG to generate pseudorandom sequences that successfully pass the NIST 800-22 randomness tests. Subsequently, the generated pseudorandom sequence is XORed with the plaintext image to produce the final encrypted output. The proposed scheme significantly reduces the need for transmitting large volumes of key streams by requiring only the sharing of a short key between the sender and receiver. To ensure key uniqueness, a salted hash function is employed, guaranteeing that the encryption process uses distinct key streams each time. The encryption and decryption mechanisms are straightforward, offering fast processing speeds. Experimental evaluations indicate that the encrypted images exhibit strong performance in various security analyses. 


The Gan-based PRNG is implemented using PaddlePaddle, while the experimental tests and related analyses are implemented using the Python programming language.

