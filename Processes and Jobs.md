# Processes and Jobs

## Listing Processes
Used **ps aux** and then ran the required command.

Flag: `pwn.college{0TJiqKwxOHgpdw0qAET2wfoKOUx.dhzM4QDL0QjN0czW}`


## Killing processes
To terminate **/challenge/dont_run** so that **/challenge/run** could execute, I first found its PID using **ps -e | grep /challenge/dont_run**, which returned 73. I then executed **kill 73** to stop the process, followed by running **/challenge/run** to retrieve the flag.

Flag: `pwn.college{YALuabq-P-B4dz51rN4yaCvhVA4.dJDN4QDL0QjN0czW}`


## Interrupting processes
Ran **challenge/run** and used ctrl+c to interrupt it.

Flag: `pwn.college{cSeN8sSKtp2aKJG2WfenwVdTYLG.dNDN4QDL0QjN0czW}`


## Suspending Processes 
Ran **challenge/run**, then ctrl+z then ran the command again after which I retrieved the flag.

Flag: `pwn.college{UFwOYGvo08fZSkxKYkyMfFkZTOC.dVDN4QDL0QjN0czW}`


## Resuming Processes
Ran **challenge/run**, then ctrl+z then ran the command **fg /challenge/run** after which I retrieved the flag.

Flag: `pwn.college{QzBr8Ts-zFaZRJInWBYnaDlUP7v.dZDN4QDL0QjN0czW}`


## Backgrounding Processes
Similar to before, I used **bg /challenge/run**, after which I ran **/challenge/run** again.

Flag: `pwn.college{4XpNHtpyExRO1qNYyWDsCPSXsDv.ddDN4QDL0QjN0czW}`


## Foregrounding Processes
This challenge involved first suspending **/challenge/run** using **Ctrl-Z**, then resuming it in the background with **bg /challenge/run**, and finally bringing it back to the foreground using **fg /challenge/run**.

Flag: `pwn.college{cPj1JJSCLvExj4DTUDJ7ZaKB2fP.dhDN4QDL0QjN0czW}`



## Starting background processes
To run **/challenge/run** in the background and retrieve the flag, I simply executed **/challenge/run &**.

FLag: `pwn.college{kF57SOiqKtKCVFo3WX2BHmjiHgp.dlDN4QDL0QjN0czW}`


## Process Exit Codes
To obtain the exit code of **/challenge/get-code**, I executed it, and it terminated with an error code. I then ran **echo $?**, which returned *236*. Subsequently, I passed this code as an argument to **/challenge/submit-code 236** and successfully retrieved the flag.

Flag: `pwn.college{MDSv5E7bRSVcMRU5PRB7t_qCEt7.dljN4UDL0QjN0czW}`
