# HALIC-High-Availability-Lossless-Image-Compression-
New Ultra Fast Lossless Image Codec
This study, especially large-sized photographs (RGB 24 bit) are targeted, but also suitable for other types of images. I tried to find the middle way for all. Fully one thread is running and SIMD, ASM or GPU is not used. Windows and Linux were compiled with GCC and Clang. Completely independent blocks and sub-channels are coded. Therefore, it can be easily used as multithread (per block and channel). The version can work as multithread after 0.7. No error correction or content modeling method was used in the estimation process. Therefore, there are many residual data that needs to be compressed. PPM and PNM are currently supported as input. HALIC uses ANS(FSE) as an entropy encoder.
