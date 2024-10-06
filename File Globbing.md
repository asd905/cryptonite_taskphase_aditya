# File Globbing


## Matching with *
I used  cd /ch* to cd into challenge while staying under 4 characters. Then I used **./run**.

Flag: `pwn.college{wfNPQRCOuoXWMETCO_VuGzP5ymz.dFjM4QDL0QjN0czW}`


## Matching with ?
Used **?** in place of 'c' and 'l' to cd into **challenge**.

Flag: `pwn.college{4NZcOw_pyF6Oi4uU33eFb8DzqG8.dJjM4QDL0QjN0czW}`


## Matching with []
**cd**ed into /challenge/files. Then used **/challenge/run file_[absh]** to find the flag from the possible 4 files.

Flag: `pwn.college{UBHhhWK4KcqRCt48yLW1a6vjh6G.dNjM4QDL0QjN0czW}`

## Matching paths with []
Searched for **file_[absh]** using the absolute path **/challenge/files** as an argument to **/challenge/run**.

Flag: `pwn.college{cgiqeWYbLrdlNHG8wYn1rCGMBmZ.dRjM4QDL0QjN0czW}`



## Mixing Globs
Since less than 6 characters were to be used in the argument, I used [cep]* which gave the flag.

Flag: `pwn.college{o7Esh6vUJniWiZKPc8xAVZpW9eE.dVjM4QDL0QjN0czW}`


## Exclusionary Globbing
Used [!pwn]* to look for files not starting with p, w, or n and ran it.

Flag: `pwn.college{gRRjz_Spd9WUX_wtZ8_kdAHo855.dZjM4QDL0QjN0czW}`

