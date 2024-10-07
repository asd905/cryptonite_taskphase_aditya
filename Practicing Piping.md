# Practicing Piping

## Redirecting Output
Used > to redirect **echo PWN** to **COLLEGE**.

Flag: `pwn.college{gt1-qEsmNJHRG-Gzy1iQhUZTDlA.dRjN1QDL0QjN0czW}`


## Redirecting More Output
Redirected */challenge/run* to **myflag**.

Flag: `pwn.college{ID5LsFWlugt7zHbf133yKVroa9D.dVjN1QDL0QjN0czW}`


## Appending Output
I appended the output of */challenge/run* to *~/the-flag*. Then, I **cat**ed the file.

Flag: `pwn.college{QhmWGB9MDlL_HGdS7RnBYVVZt9P.ddDM5QDL0QjN0czW}`


## Redirecting Errors
Used 1> to redirect the flag and 2> to redirect the error to the respective files.

Flag: `pwn.college{0vl3QJ8YpM5SL_qlNMs1Ajo1sut.ddjN1QDL0QjN0czW}`


## Redirecting Input
First, I had to use **echo** and 1> to redirect **COLLEGE** to **PWN**. After that, since I had to redirect **PWN** to */challenge/run*, I used <. That gave me the flag.

Flag: `pwn.college{0zv0ug9ZouWmUBv9gQ2zBOQLNgO.dBzN1QDL0QjN0czW}`


## Grepping Stored Results
First, I redirected */challenge/run* to */tmp/data.txt*. Since I had to grep for the flag, I used the **grep** command with the argument 'pwn.college' to find the flag, since the flags always begin with the sub-string 'pwn.college'.

Flag: `pwn.college{MX0SqZ5XKjOGjA9kXgi2KfgJ5pw.dhTM4QDL0QjN0czW}`


## Grepping Live Output
Grepped */challenge/run* with |, for the argument 'pwn.college' for the same reason as above.

Flag: `pwn.college{wp5cbaQokQbDXZkoNsy2ghvr9OI.dlTM4QDL0QjN0czW}`


## Grepping Errors
Combined stdout and stderr using **2>&1** and grepped for 'pwn.college' with |.

Flag: `pwn.college{QiWXbQtfA3GHy6wI7EHjj5axsOk.dVDM5QDL0QjN0czW}`


## Duplicating Piped Data with tee
First, I did **/challenge/pwn | tee intercepted_output | /challenge/college** and **cat intercepted_output** to find the argument required for --secret. After finding the argument, I used **/challenge/pwn --secret [ARGUMENT] | tee /challenge/secret | /challenge/college**, and found the flag.

Flag: `pwn.college{UOftD7i27q2S2o1Ons98GS5PEBT.dFjM5QDL0QjN0czW}`


## Writing to Multiple Programs
Ran the command **/challenge/hack | tee >(challenge/the) >(challenge/planet)** to duplicate **/challenge/hack** into both required files.

Flag: `pwn.college{kghU1rCuzrVWAhnWGNyGhm_1lNO.dBDO0UDL0QjN0czW}`


## Split-Piping stderr and stdout
Use **command > >(program1) 2> >(program2)** to redirect **stdout** to **program1** and **stderr** to **program2**.


Flag: `pwn.college{gItQE3sFTlzNeXWy9FZ850DeD9P.dFDNwYDL0QjN0czW}`