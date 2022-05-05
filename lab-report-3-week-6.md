# Lab Report 3
## Streamlining ssh Configuration
### My `.ssh/config` file, I edited the file using Notepad.
![My ssh config file in directory](r3config.png)
![open with notepad](notepadconfig.png)
![opened in notepad](notepadopenconfig.png)
### The ssh command logging me into my account using the alias ieng6
![ssh command to account using alias](r3sshconfigtoserversuccess.png)
### An scp command copying a file to my account using the alias I chose.
![scp copying file to account using alias](r3scpwithconfig.png)
## Setup Github Access from ieng6
### Location of public key in Github and in user account
![location of public key in Github](publickeygithub.png)
The location of my public key in Github
![location of public key in my user account](pubprivlocuser.png)
![location of public key in my user account](r3config.png)
The location of my public key `id_rsa.pub` in my user account
### Location of private key in user account
![location of private key in user account](pubprivlocuser.png)
![location of private key in user account](r3config.png)
The location of my private key `id_rsa` in my user account
### Running `git` commands to commit and push change to Github while logged in ieng6
![running git commands to commit/push changes in ieng6 to Github](commitandpush.png)
[link to resulting commit](https://github.com/canitry/markdown-parser/commit/08bda667b47647ea90cca53dd0f9467636653371)
## Copying whole directories with scp -r
### Copying whole markdown-parse directory to my ieng6 account
![copying markdown-parser directory to ieng6 account](beginningofscpr.png)
...
![copying markdown-parser directory to ieng6 account](endofscpr.png)
### Logging into my ieng6 account after copying directory and compiling and running tests from my repository
![login and compiling and running repo in ieng6 account](runningonieng6.png)
### Combining `scp`, `;`, and `ssh` to copy the whole directory and run the tests in one line.
I was unable to do this, and the TA's were unable to provide an answer, I both used direct commands and makefile but it failed because it could not find symbol such as Path.of or readString, I have posted on Piazza and will update the below images if it is successful:
#![using scp;ssh to copy whole dir and runs tests in one line]()
Failing with normal method
![Normal method](normalfirstfail.png)
![Normal method](normallastfail.png)
Failing with make test and showing that running the same commands while logged into ieng6 works
![makefile method](makefilefail.png)
![makefile method](makefilesuccessieng6.png)