# 060-Acquisition

## Evidence acquisition

* Analysing the original evidence could modify or even destroy the evidence
* Necessary to acquire the original digital evidence in a manner that `protects and preserves` the evidence

## Types of acquisition

* Live data acquisition
  * Acquisition of volatile data (live forensics)
* Static data acquisition
  * Acquisition of non-volatile data

## Live forensics

* System information
* Current configuration and running state of computer
* Volatile system information
* Network information

## Static data acquisition

* Non-volatile information
* Files / data in storage media
* Data includes slack space, swap files, unallocated drive spaces

## The need of media duplication

* Disk or media duplication is at the core of computer forensics process
* Necessary to create an `exact` copy of the original disk/ media for analysis because of the volatility of the data on the disk and potential that evidence could be modified or destroyed during handling and analysis

## Simple backup / copy...

* Only copied the active data
  * i.e., All the files you can see
  * Not include slack, residue, deleted files
  * May not capture the timestamp of the data

## Bit stream image

* To be complete and accurate, the copy should be a `bit-by-bit clone` of the original disk, called a `bit stream image`
* A bit stream copy is recording every single bit (0 or 1) of data that resides on a storage device
* The bit stream copy allows copying of working files, and also `hidden, erased, fragmented, corrupted, temporary and special attribute files`

## Preparation of the media
* A brand new media / clean media
* Media sanitisation
  * Clear
    - Logical techniques using standard read-write commands
  * Purge
    - Physical / logical techniques to make target data recovery infeasible by state-of- the-art laboratory techniques
  * Destroy
    - Use of state-of-the-art laboratory techniques but result in inability to use the media for data storage (e.g., cross-cut shredding)

## Write protection

* Write protection should be initiated to preserve and protect the original evidence
* A `write blocker` is any tool that permits `read-only` access to data storage devices without compromising the `integrity` of the data
* Two types of write blockers:
  * Hardware write blockers
  * Software write blockers

## Disk imaging
* Disk imaging can be done using software
  * Forensics application suite
    - Examples: EnCase® Forensic, AccessData® FTK®
  * Forensics imaging utility
    - Examples: EnCase® Forensic Imager, AccessData® FTK® Imager, dd

## AccessData® FTK® Imager

* A data preview and imaging tool that allows quickly assess of digital evidence
* Allows creating forensic sound images of different media
  * Makes a bit-by-bit duplicate of the media
* The forensic image is identical in every way to the original, including file slack and unallocated space or drive free space

## Integrity of disk copy

* Have to prove that the disk image is `exactly` the same as the original evidence
* Comparison of a digital fingerprint
* `Hashes` of the original evidence and disk image should be created

## Hashing

* Hashing is a mathematical process (via an algorithm) that produces a unique value (hash value) that is essentially the digital "fringerprint" or "DNA" of a particular file, piece of media, etc
* This digital fingerprint can be used to compare the original evidence to the forensic image
  * These two values should match exactly

## Types of hashing algorithm

* Common hash functions:
  * Message Digest 5 (MD5)
  * Secure Hash Algorithm (SHA-1) and SHA-2

## Use of hashing

* Hash values can be used throughout the digital forensic process
  * Used after the cloning process to verify that the clone is indeed an `exact duplicate`
  * Used as `an integrity check` at any point
  * Used to `identify` specific files
* Recorded throughout the chain of custody