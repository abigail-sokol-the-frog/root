# root
A less bloated sudo that is probably insecure and a horrible idea to ever use.

Will, of course, only work on linux.

Setup
    
    Compile, possibly with "gcc root.c -o root -lcrypt"
    Then make sure to set the setuid bit first
        - possibly with running "chown root:root root" then "chmod +s root" as the user root)
    Then either set an alias in .bashrc or move the file to /bin/root

Usage:
    
    root $command (arguments)

Disclaimer
    
    I'm not sure if it is safe or not, so use at your own risk.
    Only users in sudo group will be able to use command

Help
    
    If you see a security flaw please let me know.

Possible Bugs
    
    - A username over 100 characters in group sudo may cause an infinite loop
