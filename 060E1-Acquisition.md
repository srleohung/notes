# 060E1-Acquisition

## 1. Why it is necessary to create a duplication of the original media during the forensic investigation process?
<details>
<summary>Answer</summary>
<p>
Digital evidence are highly fragile, analyzing the original evidence could easily altered, damaged or even destroyed the evidence.
To prevent accidental or intentional manipulation of the original evidence, it is necessary to create a duplication of the original media during the forensic investigation process. The resulted forensic image is identical in every way to the original, not only including the working files, but also hidden, erased, fragmented, corrupted, temporary and special attribute files.
This allows storing the original media away, safe from harm while the investigation proceeds using the disk image.
</p>
</details>  

## 2. Assume that you received an external portable hard drive from the evidence collection team of your company, and you are assigned to create a copy of the hard drive.
### (a) Name a software that can be used to image the data in the hard drive.
<details>
<summary>Answer</summary>
<p>
AccessData FTK Imager.
Several tools are available to image data, such as AccessData FTK Imager, EnCase Forensic Imager, and the utility dd in Unix/Linux.
</p>
</details>  

### (b) You are going to use the software you mentioned in (a) for creating the copy. Write down the steps, including the hardware and/or software you will use, for performing the task.
<details>
<summary>Answer</summary>
<p>

1. Connect the portable hard drive to a hardware-based write blocker.
2. Connect the hardware-based write blocker to the computer.
3. Start FTK Imager to create a forensic image of the hard drive.
4. Check the output of FTK Imager to ensure the resulted forensic image is exactly the same as the original source.
5. Start a software-based write blocker application on the computer, and start the write-blocking function.
6. Connect the portable hard drive to the computer.
7. Start FTK Imager to create a forensic image of the hard drive.
8. Check the output of FTK Imager to ensure the resulted forensic image is exactly the same as the original source.
</p>
</details>  

### (c) How can you verify that during the process of media duplication, the original media is unchanged?
<details>
<summary>Answer</summary>
<p>
It is necessary to generate hash reports of the original media, which is used as a benchmark to prove the integrity of the evidence. Algorithms such as Secure Hash
Algorithm (SHA-1) and SHA-2, or Message Digest 5 (MD5) can be used as the hash function.
When the portable hard drive is imaged, a drive hash and an image hash are generated for verification. The drive hash should match the hash reports of the original media to prove that the original media is unchanged during the process of media duplication.
</p>
</details>  