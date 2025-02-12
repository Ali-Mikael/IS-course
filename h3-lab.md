# Linux (X)

Installing linux. 
- Download to ISO file. Configure a virtual hard disk (as well as other system settings).
- Start the machine, begin configurations and downloading.
- After the machine is ready, delete CD and put hard disk as boot option #1.
- Boom, now you have linux on your machine.
- Pretty straighforward!


## Can't fish (A)
Before and after disconnecting from the internet.
<img width="805" alt="Screenshot 2025-02-06 at 13 05 27" src="https://github.com/user-attachments/assets/803c55b5-472c-4237-8af7-3e90b3ff88c6" />

A succesfull ping command reply shows that we are infact connected to the internet. 
Not getting a successfull ping commmand reply could mean either of three things:
1. we have a connection problem
2. the end device we're trying to connect to has connection problems.
3. Or that there are problems somewhere inbetween

Well, this time it's pretty simple to know the cause, as we ourself disabled the network, and this was just a quick way to confirm that it worked. 




## Port scanning (B-C)
I port scanned my linux VM (localhost). (While being disconnected from the internet)
<img width="1028" alt="Screenshot 2025-02-06 at 13 15 03" src="https://github.com/user-attachments/assets/95e52177-22a6-4068-8d91-7b3cb115e7a2" />

-Because all 1000 scanned ports reported to be in ignored states, i came to the conclusion that either the FW is blocking the scan, or that they really are close.

**Now i actived the internet back up, plus i activated the ssh server**

<img width="1020" alt="Screenshot 2025-02-06 at 13 27 54" src="https://github.com/user-attachments/assets/f34f93c8-1e42-40d2-94e4-da33abe477a2" />
I then ran the command again


<img width="1028" alt="Screenshot 2025-02-06 at 13 28 39" src="https://github.com/user-attachments/assets/30ace016-1555-467d-a392-118532615c94" />

- This time a got a lot more information from the scan. 
- So my previous guessing game was partially right, there just wasn't any ports open. 
- Now that the ssh port was open, the scan was succesfull in gaining information about the port, what service is was runnning, plus the operating system and other details about the VM. 
- Very interesting stuff, i was surprised how only one open port could give this much information.


*Thoughts:*
- Only one open port on a computer gives us a whole lot of information about the machine with the nmap tool.
- When we figure out the target OS/kernel/machine, we can look for other vulnerabilites for that specific system, and tailor an attack.
- This exercise gave me some valid insight into the first step of an attack, and why it is crucial: recoinnaissance. 








## OverTheWire (D)
> Premise: log into the game server using ssh on port 2220. 
>
> Using various methods,
> locate and open the correct file, aquire the password, and move on to the next level.


**Level 1:** 
- Getting to the level one, requires a password from level0, which is stored in the home directory in a file called readme. The password for bandit0, is bandit0
<img width="1017" alt="Screenshot 2025-02-06 at 13 39 03" src="https://github.com/user-attachments/assets/cbc4fa39-32f9-47ce-8e4d-189f3b75eae5" />

**Level 2:**
- The password for this level was located in a file called -. Pretty easy to get around it with the command ./-
- Starting from the home directory and putting the forwardslash, tells the system now it's time for the name.
<img width="864" alt="Screenshot 2025-02-06 at 13 42 51" src="https://github.com/user-attachments/assets/4df84343-39c4-4928-8507-a565ff4c546c" />

**Level 3:**
- Same idea as last time.
- Escaping the spaces in the filename using ""
<img width="769" alt="Screenshot 2025-02-06 at 13 44 39" src="https://github.com/user-attachments/assets/1e295bc7-24f5-408b-9f50-21603d4ea3f4" />


**Level 4:**
- For this level, the password was in a hidden file, in the inhere directory. Just use the ls -a to discover it.
- For ease of typing open it with cat ...*
<img width="665" alt="Screenshot 2025-02-06 at 14 12 42" src="https://github.com/user-attachments/assets/946ae2ab-efec-4ffd-bb43-316311b4e87c" />



**Level 5:**
- The password for this level was in the only human readable file inside inhere directory
- i used a combination of find (searching for the file) and grep (to filter human-readables) to locate the file. 
<img width="979" alt="Screenshot 2025-02-06 at 14 10 08" src="https://github.com/user-attachments/assets/41edb0fa-16ac-4258-a63b-3353044ac3ca" />

