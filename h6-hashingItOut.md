# Applied cryptography (x)
> Applied Cryptography: Protocols, Algorithms and Source Code in C, 20th Anniversary Edition - Bruce Schneier

**Chapter 2.3 / One-way function**
- One way functions are easy to compute, but infeasible to reverse.
- The function enrypts plain text data --> into an unreadable string.
- They play a central role in public-key cryptography, as the functions are extremely challenging to reverse, without the private-key.
- The afore mentioned method is called a *trapdoor one-way function*
  - The public-key (one-way function) is used to encrypt the data, and can only be decrypted using a corresponding private-key (the secret trapdoor).

  
**Chapter 2.4 / One way-hash function**
- The mechanics of a one-way hash function is pretty straight forward
  - Take a variable size string = **pre-image** --> run it through the mathematical function --> out comes a fixed-length string of various letters, characters and nuumbers = **hash value**
- The key thing here, is that it's easy to calculate the hash value from the pre-image,
but it's unreasonable, or extremeley challenging at best, to get a pre-image to match a certain hash value.
- A good one-way hash function is also collision free: meaning it's extremely challenging to produce 2 pre-images with the same hash value.
- **MAC (Message Authentication code)**
  - The use of a hash function in conjuction with a secret key.
  - Meaning: you add a secret key to the data to be hashed, and so only the one with the secret key can verify the authenticity/integrity of the data.




# Hashcat (A)
- --> I fired up the kaliVM
- --> Updated the system
- --> Downloaded the required packages (wget, hashid & hashcat), but as it turns out, i already had them installed, which the system kindly let me know.
- I started off by using wget to download a file from github with over 14 million passwords.
  - <img width="1100" alt="Screenshot 2025-03-01 at 14 10 44" src="https://github.com/user-attachments/assets/82260fa7-7984-422e-a9e9-db98aa940230" />
  - <img width="467" alt="Screenshot 2025-03-01 at 14 11 05" src="https://github.com/user-attachments/assets/98a1cde9-b9ff-4fbc-8a52-210650e8d855" />
- This is a good place to start hash comparing.
- The file was obviously compressed, so i decompressed, and out came a file: *rockyou.txt*
- I then used the *hashid* tool to figure out the type of the hash we were up against. It gave me many answers, but I went with the md5 as it was the most commong out of the other top 2.
  - <img width="638" alt="Screenshot 2025-03-01 at 14 23 57" src="https://github.com/user-attachments/assets/4191891f-6595-4966-b614-59a642c08640" />
- Now we had something to work with, so I went ahead and used the following command with the *hashcat* tool, in order to crack the hash.
- **$hashcat -m 0 '6b1628b016dff46e6fa35684be6acc96' rockyou.txt -o solved.txt** (explanation for this command will be discussed later)
- Below was the output we derived.
  - <img width="980" alt="Screenshot 2025-03-01 at 14 32 52" src="https://github.com/user-attachments/assets/fc4428cd-7321-4401-9b9c-e56d41ec644c" />
- The hashcat tool goes through the provided password-list, hashesh the passwords, and compares them to our hash, in case of a match, the program stops and returns the value to our solved file. 




# Cracking the password (B)
- Get the password hash you want to crack : in our case = *d595b2086532422bbe654bc07ea030df*
- Use *hashid* to determine which type of hash we're up against.
  - <img width="656" alt="Screenshot 2025-03-01 at 14 42 04" src="https://github.com/user-attachments/assets/d28e1478-629e-4ebe-bf3a-358cf262e76c" />
- Since md5 is the most popular out of the first three, we'll go with md5.
- Decide on a dictionary of your choice : in our case *rockyou.txt* (the file with 14million passwords we downloaded earlier)
- Make use of the *hashcat* tool, with the following command:
  - <img width="1028" alt="Screenshot 2025-03-01 at 15 04 22" src="https://github.com/user-attachments/assets/3d7f0f54-78a5-4c5a-af23-e1b01147c5e6" />
- And get to cracking!
- The command works in the following way:
  - The '-m 0' specifies the mode, with 0 = md5 here.
  - Then we simply specify the hash we wan't to 'crack' (we are actually just hashing words from the provided dictionary and doing a simple comparison operation)
  - The rockyou.txt is simply the file we use for comparison.
  - And lastly the '-o solved.txt' just tells the program where to store a possible answer. with -o indicating output and the latter being the text file where to store it. 



# Sources
> Applied Cryptography: Protocols, Algorithms and Source Code in C, 20th Anniversary Edition - Bruce Schneier
> https://terokarvinen.com/2022/cracking-passwords-with-hashcat/









