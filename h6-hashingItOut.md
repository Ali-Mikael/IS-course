# Applied cryptography (x)
> Applied Cryptography: Protocols, Algorithms and Source Code in C, 20th Anniversary Edition - Bruce Schneier

**Chapter 2.3 / One-way function**
- One way functions are easy to compute, but infeasible to reverse.
- They play a central role in public-key cryptography, as the functions are extremely challenging to reverse, without the private-key.
- The afore mentioned method is called a *trapdoor one-way function*
  - The public-key (one-way function) is used to encrypt the data, and can only be decrypted using a corresponding private-key (the secret trapdoor).

  
**Chapter 2.4 / One way-hash function**
- The mechanics of a one-way hash function is pretty straight forward
  - Take a variable size string (pre-image) --> run it through the mathematical function --> out comes a fixed-length string (hash value)
- The key thing here, is that it's easy to calculate the hash value from the pre-image,
but it's unreasonable, or extremeley challenging at best, to get a pre-image to match a certain hash value.
- A good one-way hash function is also collision free: meaning it's extremely challenging to produce 2 pre-images with the same hash value.
- **MAC (Message Authentication code)**
  - The use of a hash function in conjuction with a secret key.
  - Meaning: you add a secret key to the data to be hashed, and so only the one with the secret key can verify the authenticity/integrity of the data.




# Hashcat (A)
I Fired up the kaliVM and updated the system, as it turns out, i had all the required programs already installed (wget, hashid & hashcat) so let's just get straight to cracking. 


- I started off by using wget to download a file with over 14 million passwords.
  - <img width="1100" alt="Screenshot 2025-03-01 at 14 10 44" src="https://github.com/user-attachments/assets/82260fa7-7984-422e-a9e9-db98aa940230" />
- This is a good place to start trying out our hash-solving skills. The file was obviously compressed, so i decompressed it and removed the original
  - <img width="467" alt="Screenshot 2025-03-01 at 14 11 05" src="https://github.com/user-attachments/assets/98a1cde9-b9ff-4fbc-8a52-210650e8d855" />
- I then used the hashcat with the md-5 mode i deduced form hashid. I
  - <img width="980" alt="Screenshot 2025-03-01 at 14 32 52" src="https://github.com/user-attachments/assets/fc4428cd-7321-4401-9b9c-e56d41ec644c" />


  - something nice
    - The output <img width="980" alt="Screenshot 2025-03-01 at 14 32 52" src="https://github.com/user-attachments/assets/3b93b57c-1ec7-4cef-a46c-9a2cc1e15e7b" />





### Cracking the password (B)
- Get the password hash you want to crack : *d595b2086532422bbe654bc07ea030df*
- Use hashid to determine which mode it is using
  - <img width="656" alt="Screenshot 2025-03-01 at 14 42 04" src="https://github.com/user-attachments/assets/d28e1478-629e-4ebe-bf3a-358cf262e76c" />
- Since md5 is the most popular out of the first three, we'll go with md5 (0)
- Decide on a dictionary of your choice : in our case *rockyou.txt* (the file with 14million passwords we downloaded earlier)
- Make use of the hashcat tool, with the following command
  - <img width="1028" alt="Screenshot 2025-03-01 at 15 04 22" src="https://github.com/user-attachments/assets/3d7f0f54-78a5-4c5a-af23-e1b01147c5e6" />
- And get to cracking!
- The command works in the following way
  - The '-m 0' specifies the mode, meaning the md5 we deduced earlier by using the hashid command.
  - Then we simply specify the hash we wan't to 'crack' (we are actually just hashing words from the list and doing a simple comparison operation
  - The rockyou.txt simply specifys the file we wan't to use as our dictionary base.
  - And lastly the '-o <target>' just tells the program where to store the output/answer/crackedpassword/




