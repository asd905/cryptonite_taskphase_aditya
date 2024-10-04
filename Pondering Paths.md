# Pondering Paths

## The root
It was specified that the `pwn` file was in the root. I used the absolute path to get the flag.

Flag: `pwn.college{AaBbaoJloitDOxTLt3he079n7jD.dhzN5QDL0QjN0czW}`


## Program and Absolute Paths
It was specified that the file to run was in the challenge directory. I used the absolute path to get into the challenge directory and ran the 'run' file. 

Flag: `pwn.college{App3ydiLRRkEGjnNKmJse1O1aAw.dVDN1QDL0QjN0czW}`


## Position Thyself
The correct directory to be opened was **/var/log**. The *cd* command was used to go to that directory and then the absolute path **/challenge/run** was used.

Flag: `pwn.college{QH9cNhX0TypZyD8rF3D7-qJuZzl.dZDN1QDL0QjN0czW}`


## Position Elsewhere
As above, I **cd**ed to the directory */var* and got the flag.

Flag: `pwn.college{E8SdKmUQSMunrDtJXd_XJ0i5Ufo.ddDN1QDL0QjN0czW}`


## Position yet Elsewhere
As above, I **cd**ed to the directory */tmp* and got the flag.

Flag: `pwn.college{AcAya4SRcJCG4wo6GriDIEXZMIl.dhDN1QDL0QjN0czW}`


## Implicit relative paths, from /
Since relative path was to be used, I **cd**ed to the / directory. Then I used the implicit command *challenge/run* to get the flag.

Flag: `pwn.college{8JsMJmLUw-v-U3Qlm42mUiIgx_l.dlDN1QDL0QjN0czW}`


## Explicit relative paths, from /
Since relative path was to be used, I **cd**ed to the / directory. Then I used the explicit command *./challenge/run* to get the flag.

Flag: `pwn.college{I67IjTl9EbXJs0II2tQxrWB030D.dBTN1QDL0QjN0czW}`


## Implicit relative paths
First, I **cd**ed to the */challenge* directory. Since it was given that implicit path would not work as a safety measure, I used the explicit path to run the file.

Flag: `pwn.college{MKRUZo_K6cyI0aECvGwlHIobxAQ.dFTN1QDL0QjN0czW}`


## Home Sweet Home
I specified the argument **~/e** to the /challenge/run command. This was an absolute path to the home directory as required. The command wrote a copy and read the flag back.

Flag: `pwn.college{sOFnnVjDvPMQWpRjcs3rt_is4SC.dNzM4QDL0QjN0czW}`