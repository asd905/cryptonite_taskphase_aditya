# Pondering PATH


## The PATH Variable
Here, I used **PATH=""** to blank the path. 

Flag: `pwn.college{QxfiFxCDgpP5C_j6f2v6xOCtPgL.dZzNwUDL0QjN0czW}`


## Setting PATH
First, I set the PATH variable to include the **/challenge/more_commands/** directory. Then, I invoked **/challenge/run**.

Flag: `pwn.college{8xLuK9Kuuewtk1rpnghpuxbAaTG.dVzNyUDL0QjN0czW}`


## Adding Commands
I created the win script and made it executable just as before. I checked my current PATH variable to see the default directories using **echo $PATH**. Then I set the path to include the directory of the win script. Then, I ran **/challenge/run**.

Flag: `pwn.college{MWCi_90VUyNeZAQOF9tGSB7ADl1.dZzNyUDL0QjN0czW}`


## Hijacking Commands
In this, to prevent the deletion of the flag file, I created a custom *rm* script. By modifying the PATH variable, I ensured that when I run **/challenge/run**, and attempt to call *rm*, it uses my version instead, safeguarding the flag.

Flag: `pwn.college{QxfiFxCDgpP5C_j6f2v6xOCtPgL.dZzNwUDL0QjN0czW}`