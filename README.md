# OverTheWire-Bandit
<p align="center">
    <img src = "Assets/overthewire-logo-1.png"/>
</p>

<!--![](Assets/overthewire-logo-1.png)-->

This repository contains a walkthrough guide to completing the [Bandit](http://www.overthewire.org/wargames) levels in the OverTheWire wargames.

This repository serves as:
1) Documentation of my methods and thought process as I solve each level.
2) Revision guide based on the key takeaways from solving each challenge.

Each level of the walkthrough guide summarises the:
1) Level Goal (taken verbatim from what's given on the site)
2) Key Takeaways

# Walkthrough Guide
**Bandit Level 0**  
**Level Goal**: The goal of this level is for you to log into the game using SSH. The host to which you need to connect is bandit.labs.overthewire.org, on port 2220. The username is bandit0 and the password is bandit0.

* Commands: 
    - `ssh bandit0@bandit.labs.overthewire.org -p 2220`
    - `exit`
* Password for Level 0: `bandit0`

**Bandit Level 0 → Level 1**  
**Level Goal**: The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. *Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.*

* Commands: 
    - `ssh bandit0@bandit.labs.overthewire.org -p 2220`
    - `cat readme`
    - `exit`
* File: `readme`
* Password for Level 1: `NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL`

**Bandit Level 1 → Level 2**  
**Level Goal**: The password for the next level is stored in a file called - located in the home directory

* Commands: 
    - `ssh bandit1@bandit.labs.overthewire.org -p 2220`
    - `cat ./-`
    - `exit`
* File: `-`
* Password for Level 2: `rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi` 

**Bandit Level 2 → Level 3**  
**Level Goal**: The password for the next level is stored in a file called spaces in this filename located in the home directory

* Commands: 
    - `ssh bandit2@bandit.labs.overthewire.org -p 2220`
    - `cat spaces\ in\ this\ filename`
    - `exit`
* File: `spaces in this filename`
* Password for Level 3: `aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG` 

**Bandit Level 3 → Level 4**  
**Level Goal**: The password for the next level is stored in a hidden file in the inhere directory.

* Commands: 
    - `ssh bandit3@bandit.labs.overthewire.org -p 2220`
    - `cat inhere/.hidden`
    - `exit`
* File: `.hidden`
* Password for Level 4: `2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe`

**Bandit Level 4 → Level 5**  
**Level Goal**: The password for the next level is stored in the only human-readable file in the inhere directory. *Tip: if your terminal is messed up, try the “reset” command.*

* Commands: 
    - `ssh bandit4@bandit.labs.overthewire.org -p 2220`
    - `file inhere/*`
    - `cat inhere/-file07`
    - `exit`
* File: `-file07` *ASCII text*
* Password for Level 5: `lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR`

**Bandit Level 5 → Level 6**  
**Level Goal**: The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

    + human-readable
    + 1033 bytes in size
    + not executable

* Commands: 
    - `ssh bandit5@bandit.labs.overthewire.org -p 2220`
    - `find ./* -type f -readable -size 1033c ! -executable`
    - `cat ./inhere/maybehere07/.file2`
    - `exit`
* File: `./inhere/maybehere07/.file2`
* Password for Level 6: `P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU`

<!--
-----------------------
**Bandit **  
**Level Goal**: 

* Commands: 
    - `ssh bandit@bandit.labs.overthewire.org -p 2220`
    - ``
    - `exit`
* File: ``
* Password for Level : ``
-->