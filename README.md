# 32-bit-challenge

A challenge to see how much structured information we can fit in a single 32bit integer


## Some introduction

How much of structured information can a single 32-bit word represent? 

Some examples to get your mind working:
* 1 UTF-32 Unicode code point, or up to 2 UTF-16 code units, or up to 4 UTF-8 code units
* A bit set of up to 32 continuous integers or e.g. 16 integers + 16bit offset
* a vector of 8 4-bit nibbles, eg 8 packed BCD digits
* I could go on forever... or can I?

Whoever gets the most interesting example gets the 
equivalent 100$ in digital or fiat currency of his 
or her choosing. 

I plan to do pay it on monthly 
basis as long as cool ideas keep 
flowing. 

So - put RFC-style plain text or markdown files in the repo 
in the /32 folder to get it going. I'll post my ideas regularly. 

## Basic rules

1. It has to be a single 32-bit value as a dense bitvector, 
as in 32-bit machine word.

2. Bonus points if the endianness doesn't matter when reading it from 
octet stream or there is way to detect it.

3. Bonus points if the bit pattern if all 4 octets 
are in the subset of printable ASCII.

4. Bonus points if the format has check sum and/or
error correction code embedded.

5. The last but not least it has to cover meanigful
(subset of) information of some real-world domain.
