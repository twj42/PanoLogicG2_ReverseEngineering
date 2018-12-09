# Introduction

The Pano Logic device was originally a designed as a replacement for a full fat PC based end user device, this is a class of device known as "Thin Client". An article in HackaDay in 2013 revealed that these devices basically just consist of a large Xilinx FPGA, plus some peripheral devices (USB, Ethernet, etc). This means they are largely "soft" and eminently hackable and re-purposable.

There are two main PL devices - the G1, based on a Xilinx Spartan 3 FPGA, and the G2, which uses a Spartan 6. Reverse engineering efforts were concentrated on the G2, for two main reasons - 1) the S3 is rather long in the tooth now, and 2) the physical construction of the G2 means it is much more hacker friendly (more on this later).
