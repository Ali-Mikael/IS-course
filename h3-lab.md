# Linux

Installing linux. 
- Download to ISO file. Configure a virtual hard disk (as well as other system settings).
- Start the machine, begin configurations and downloading.
- After the machine is ready, delete CD and put hard disk as boot option #1.
- Boom, now you have linux on your machine.
- Pretty straighforward!



## Port scanning.
I port scanned my host computer.
> **This is what i found out:_**
- 998 tcp ports were close.
- The MAC address (also which manufacturer).
- Machine type
- Operating system
- Network distance

## Scanning localhost.
- Gave me the same type of information.
- After I activated the ssh server (which was already installed). This time it gave me information on which port was active for ssh.
- Additionally it gave the ssh keys.



## OverTheWire
> Premise: log into the server using ssh on port 2220. Using various commands and methods,
> locate and open the correct file, aquire the password, and move on to the next level.


**Level 1:** 
- Getting to the level one, requires a password from level0, which is stored in the home directory in a file called readme.txt


**Level 2:**
- The password for this level was located in a file called -. Pretty easy to get around it with the command ./-
- Starting from the home directory and putting the forwardslash, tells the system now it's time for the name

**Level 3:**
- Same idea as last time.
- Escaping the spaces in the filename using ""

**Level 4:**
- For this level, the password was in a hidden file, in the inhere directory. Just use the ls -a to discover it.
- For ease of typing open it with cat ...*

**Level 5:**
- The password for this level was in the only human readable file inside inhere directory
- i used a combination of find (searching for the file) and grep (to filter human-readables) to locate the file. 
