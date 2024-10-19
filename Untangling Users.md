# Untangling Users

## Becoming root with su
First, I ran **su**, and then entered the required password **hack-the-planet**. Then, I read the flag.

Flag: `pwn.college{Q9Cou0qHEowtTFYiSCAnOLFqKC0.dVTN0UDL0QjN0czW}`

## Other users with su
Since I had to switch to the user *zardus*, I ran **su zardus** and entered the password. Then, I ran **challenge/run**.

Flag:  `pwn.college{0Vhe2V8at3rDwwpRKTuYyoTrZaX.dZTN0UDL0QjN0czW}`


## Cracking passwords
First, I ran **john /challenge/shadow-leak** to get the password, which was *aardvark*. Then, I proceeded as before to get the flag.

Flag: `pwn.college{g2dniGlZ7Pre1DPSDXH3nAW7p2L.ddTN0UDL0QjN0czW}`


## Using sudo
In this challenge, **sudo** is utilized to execute commands with root privileges. Given that I had sudo access, I used it to read the flag by running **sudo cat /flag**.

Flag: `pwn.college{EOjFKRefMKMuQjhU7M9_RfX-6QF.dhTN0UDL0QjN0czW}`