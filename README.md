# PLCrypto: A Symmetric Cryptographic Library for Programmable Logic Controllers

This repository contains the source codes for the paper "PLCrypto: A Symmetric Cryptographic Library for Programmable Logic Controllers" in   IACR Transactions on Symmetric Cryptology, 2021. 

## A brief intro to PLCrypto

Programmable Logic Controllers (PLCs) are control devices widely used in industrial automation. They can be found in critical infrastructures like power grids, water systems, nuclear plants, manufacturing systems, etc. This paper introduces PLCrypto, a software cryptographic library that implements lightweight symmetric cryptographic algorithms for PLCs using a standard PLC programming language called structured text (ST). To the best of our knowledge, PLCrypto is the first ST-based cryptographic library that is executable on commercial off-the-shelf PLCs. PLCrypto includes a wide range of commonly used algorithms, totaling ten algorithms, including one-way functions, message authentication codes, hash functions, block ciphers, and pseudo-random functions/generators. PLCrypto can be used to protect the confidentiality and integrity of data on PLCs without additional hardware or firmware modification. This paper also presents general optimization methodologies and techniques used in PLCrypto for implementing primitive operations like bit-shifting/rotation, substitution, and permutation. The optimization tricks we distilled from our practice can also guide future implementation of other computationheavy programs on PLCs. To demonstrate a use case of PLCrypto in practice, we further realize a cryptographic protocol called proof of aliveness as a case study. We benchmarked the algorithms and protocols in PLCrypto on a commercial PLC, Allen Bradley ControlLogix 5571, which is widely used in the real world. Also, we make our source codes publicly available, so plant operators can freely deploy our library in practice.

# Files

All ACD files in the source codes folder require a special vendor software (Studio 5000) to open. To facilitate readers with no access to Studio 5000, we provide the text version of the source codes in the "txt code" subfolder. Notice that tag declarations and PLC system settings are only visible in the ACD files. Detailed settings can also be seen in the paper.

Please also refer to "PLCrypto Manual.pdf" in the repository to see how to use the PLCrypto library. The test vectors we used in validating our implementations are in the "test vectors.doc" file. 

# Reference
1. [PLCrypto: A Symmetric Cryptographic Library for Programmable Logic Controllers, Z. Yang, Z. Bao, C. Jin, Z. Liu, and J. Zhou. (2021) In IACR Transactions on Symmetric Cryptology.](https://tosc.iacr.org/index.php/ToSC/article/view/9178) (Open Access)
