# OverTheWire-Bandit-Level-3-README.md

# Bandit Level 2-3
**Platform:** OverTheWire (Bandit)  
**Date:** 2025-09-24  
**Difficulty:** Beginner 
**Objective:** The goal of this level is to find the password for the next level (level 3-4). It is in a file called "--spaces in the filename--"

## Steps
1. SSH into the server (not shared here).  
2. Checked files with `ls` (ls is a command to list the file(s)). A file named "--spaces in the filename--" is present.
3. Tried reading a file using `cat` (cat is a command to read the file(s) but didn't open it
4. I also used the knowledge from the previous level, using different combinations, I kept getting an error message.
5. Googled what kind of file "--spaces in filename--" is, found out it's another special kind of file, and using the "cat --" directly, the terminal will see this as options
5. After research, I then used one of the methods to solve it. The file finally opened and the required password for the next level (level 3-4) was retrieved.

## Screenshots
- errors & capture.png (errors and proof (redacted))   

## Lessons
- I learnt that reading a file like "--spaces in the filename--" directly with cat won't output anything, as the terminal will see it as options.
- I learnt that you can solve this in one of 4 ways: Use -- to stop option parsing, Prefix with ./(filename) if it’s in the current directory, e.g., cat ./(filename). The ./ makes it clear you’re referring to “a file in this directory” and not parsing an option or Quote the filename e.g. cat "./filename"

