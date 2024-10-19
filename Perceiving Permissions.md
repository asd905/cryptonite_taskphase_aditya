# Perceiving Permissions

## Changing File Ownership
To change the ownership of **/flag** to **hacker**, I executed **chown hacker /flag**, and then I read its contents using **cat /flag**.

Flag: `pwn.college{kqXqaAJIK6Cr6F7EJK2IpXzImmF.dFTM2QDL0QjN0czW}`


## Groups and Files
In this case, to change the group ownership of the flag file as **hacker**, I ran **chgrp hacker /flag** and then used **cat /flag** to read the contents of the flag file.

Flag: `pwn.college{cVXstQU6viCrFqQ1jMyO7q-T9v4.dFzNyUDL0QjN0czW}`


## Fun with Groups Names
I ran **id** to find the group. Then, I proceeded as before, running **chgrp** and **cat**.

Flag: `pwn.college{ArmHpcVG-sCrS4_IC_kTcC3gOaY.dJzNyUDL0QjN0czW}`


## Changing Permissions
To make the flag readable, I added read permission for other users by executing **chmod o+r /flag**, and then I used **cat /flag** to read the contents of the flag.

Flag: `pwn.college{IhtbsC8yzXA9IXi9jfBTgf0hgGn.dNzNyUDL0QjN0czW}`


## Executable Files
To make **/challenge/run** executable, I had to add the executable permission to the user by using **chmod u+x /challenge/run**, and then I executed it.

Flag: `pwn.college{kC97CJB2rPN1nnbrvRclNFkqiwj.dJTM2QDL0QjN0czW}`


## Permission Tweaking Practice
This challenge involved changing the permissions of **/challenge/pwn** according to specific requirements, starting with running **/challenge/run**. For example, to add read permission for the user, remove execute permission from the group, and grant read and write permissions to others, I ran **chmod u+r,g-x,o+rw /challenge/pwn**.Then, I executed **chmod u+r /flag** to make it readable, followed by using **cat /flag** to read it.

Flag: `pwn.college{kk09xUE1_Yg9P45rH85sdLFkNQS.dBTM2QDL0QjN0czW}`


## The SUID Bit
In this, I ran **chmod u+s /challenge/getroot** and executed it which made it run as root. Then I ran **cat /flag** to get the flag.

Flag: `pwn.college{4y7N6WDEW4OLSTDmTZnlluxNZHt.dNTM2QDL0QjN0czW}`