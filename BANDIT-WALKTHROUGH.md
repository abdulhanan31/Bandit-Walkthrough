Bandit Walkthrough – Levels 0 to 2

-------------------------------------------------------------

Level 0 → Level 1


Objective: Log in using SSH and find the password in the readme file.

Command:

#ssh bandit0@bandit.labs.overthewire.org -p 2220
#ls
#cat readme


Output:

readme
6y2kwnwK6grgvwvpvLaa2T1cpFEKOhNR

Result: Successfully obtained the password for bandit1.

-------------------------------------------------------------


Level 1 → Level 2

Objective: Read a file named `-` in the home directory.

Commands:

#ssh bandit1@bandit.labs.overthewire.org -p 2220
#ls
#cat ./-


Output:

PK8fYLZg2hnHSz83plBL1iEPKdD3QToB

Result: Successfully obtained the password for bandit2.

--------------------------------------------------------


 Level 2 → Level 3

Objective: Read a file containing spaces in its filename.

Commands:

#ssh bandit2@bandit.labs.overthewire.org -p 2220
#ls
#cat "./--spaces in this filename--"


Output:

cat: --spaces: No such file or directory
cat: in: No such file or directory
cat: this: No such file or directory
cat: filename--: No such file or directory


Result: Successfully obtained the output for bandit3.

------------------------------------------------------


Learned the basic Linux commands:
- ssh – Connect to a remote server.
- ls – List files and directories.
- cat – Display file contents.
- exit – Close the SSH session.
