# root
A less bloated sudo that is probably insecure and a horrible idea to ever use.

Will, of course, only work on linux.

Setup
    
    Compile with "gcc root.c -o root -lcrypt -D_GNU_SOURCE"
    Then make sure to set the setuid bit first (possibly with running "chown root root root" then "chmod +s root" as the user root)
    Then either set an alias in .bashrc of move the file to /bin/root
    And your done!

Usage:
    
    root $command (arguments)

Disclaimer
    
    Probably less convientent then just using sudo, and I'm not sure if it is safe or not. So just don't use it.

Help
    
    If you see a security flaw, or happen to know how to get the suid of the process, please let me know.
