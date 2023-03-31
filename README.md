# OverTheWire-Bandit

![](/Assets/OverTheWire.jpg)

This repository contains a walkthrough guide to completing the [Bandit](http://overthewire.org/wargames/bandit/) levels in the OverTheWire wargames.

This repository serves as:
1) Documentation of my methods and thought process as I solve each level.
2) Revision guide based on the key takeaways from solving each challenge.

Each level of the walkthrough guide summarises the:
1) Level Goal (taken verbatim from what's given on the site)
2) Key Takeaways

# Walkthrough Guide
**Bandit Level 0**  
**Level Goal**: The goal of this level is for you to log into the game using SSH. The host to which you need to connect is bandit.labs.overthewire.org, on port 2220. The username is bandit0 and the password is bandit0.

* Password for Level 0: `bandit0`
* Commands: 
    - `ssh bandit0@bandit.labs.overthewire.org -p 2220`
    - `cat readme`
    - `exit`
* File: readme
* Password for Level 1: `NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL` 

**Bandit Level 0 → Level 1**  
**Level Goal**: The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. *Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.*

* Commands: 
    - `ssh bandit1@bandit.labs.overthewire.org -p 2220`
    - `cat ./-`
    - `exit`
* File: -
* Password for Level 2: `rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi` 



