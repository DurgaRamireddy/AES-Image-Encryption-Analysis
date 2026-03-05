# AES-Image-Encryption-Analysis

## Overview
This project presents a comprehensive analysis of the Advanced Encryption Standard (AES) and its application in digital image encryption. The research explores how AES can be used to secure multimedia data by transforming image content into statistically random ciphertext, preventing unauthorized access and analysis.

The study evaluates AES performance using established cryptographic and statistical metrics such as NPCR (Number of Pixels Change Rate), UACI (Unified Average Changing Intensity), entropy analysis, histogram uniformity, and correlation testing. These metrics help determine the effectiveness of AES in protecting structured image data from statistical, differential, and brute-force attacks.

The research also examines hybrid AES approaches that integrate chaotic systems, dynamic S-box generation, and pixel scrambling techniques to further enhance image encryption security.

This work was completed as part of a University of Houston cybersecurity research project, where the focus was to analyze cryptographic methods used to protect multimedia data in modern communication systems.

## Research Objectives
The primary objectives of this project were to:
- Analyze the AES cryptographic algorithm and its internal structure
- Examine how AES can be applied to image encryption workflows
- Evaluate encryption effectiveness using statistical and differential analysis metrics
- Investigate hybrid AES approaches that improve multimedia security
- Identify strengths and limitations of AES in modern multimedia environments

## AES Algorithm Overview
AES is a symmetric block cipher standardized by NIST in 2001 and is widely used across industries for secure data encryption.

AES operates on 128-bit data blocks and supports key sizes of:
- AES-128
- AES-192
- AES-256
Each encryption round includes several transformations designed to increase confusion and diffusion within the data:
- **SubBytes** - Nonlinear substitution using the AES S-box
- **ShiftRows** - Row-wise permutation to disperse byte positions
- **MixColumns** - Matrix transformation to strengthen diffusion
- **AddRoundKey** - XOR operation with a round key derived from the original encryption key
These operations collectively transform plaintext into ciphertext that appears statistically random.

## Image Encryption Workflow
To encrypt images using AES, image data must first be converted into a byte stream.

Typical workflow:
1. Convert image pixels into byte representation
2. Divide data into 128-bit blocks (16 bytes)
3. Apply AES encryption rounds to each block
4. Generate encrypted image output that resembles random noise
For RGB images, each color channel (Red, Green, Blue) may be processed separately.

## Encryption Evaluation Metrics
To evaluate encryption strength, the research examines several widely used metrics in multimedia cryptography.

**NPCR (Number of Pixels Change Rate)**
Measures the percentage of pixels that change when a single pixel in the original image is modified.
Typical secure value: ≈ 99.6% – 99.8%
**UACI (Unified Average Changing Intensity)**
Measures average intensity difference between two encrypted images.
Ideal value: ≈ 33.33%
**Entropy**
Entropy measures randomness in encrypted image data.
Ideal entropy for 8-bit images:≈ 8
AES encrypted images typically achieve entropy values around: 7.997 - 7.999
**Histogram Analysis**
Encrypted images should produce uniform histograms, indicating no visible patterns.
**Pixel Correlation**
Original images have high adjacent pixel correlation (>0.95).
Encrypted images reduce correlation to near zero.

## Hybrid AES Enhancements
Several research studies propose hybrid techniques to improve AES performance in multimedia security.

**Chaotic Map Integration**
Chaotic systems such as:
- Logistic map
- Henon map
- Lorenz attractor
can generate pseudo-random sequences for key generation or pixel permutation.

**Dynamic S-Boxes**
Dynamic S-boxes introduce variability in substitution operations, making cryptanalysis more difficult.
**Pixel Scrambling**
Techniques such as:
- Arnold Transform
- Zig-zag scanning
- Random permutation
reduce spatial redundancy before AES encryption is applied.

## Limitations
- While AES-based image encryption is highly secure, several limitations exist:
- Increased computational overhead in hybrid methods
- Complex key management for chaotic parameters
- Lack of standardization in hybrid encryption approaches
- Need for extensive security validation for new techniques

## Key Findings
This research confirms that AES remains a highly effective algorithm for multimedia encryption, demonstrating:
- Strong resistance to statistical and differential attacks
- High entropy and randomness in encrypted images
- Effective diffusion and confusion properties
- Compatibility with advanced hybrid cryptographic techniques
AES continues to play a critical role in secure multimedia communication and data protection systems.

## Skills Demonstrated
- Cryptographic algorithm analysis
- Multimedia security research
- Encryption performance evaluation
- Security metric analysis (NPCR, UACI, entropy)
- Academic cybersecurity research writing

## Tools & Technologies
- Advanced Encryption Standard (AES)
- Cryptographic analysis methods
- Statistical image analysis techniques
- Multimedia security research literature

## Author
Durga Sai Sri Ramireddy </br>
Master’s Student - Cybersecurity </br>
University of Houston

Role: **Team Lead & Primary Research Contributor**

## References
The research references multiple academic publications including IEEE, PLOS ONE, Scientific Reports, and other peer-reviewed studies on AES-based image encryption and hybrid cryptographic techniques.
