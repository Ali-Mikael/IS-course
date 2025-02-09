# Owasp 10 (X)

### A01:21 Broken Access Control
> Access control is in place, to limit authorized/unauthorized users/applications actions.
>
> Failure in access control can lead to, among other things, corruption/loss/unauthorized-access on data and bussines disruption.

**Common AC Vulnerabilites:**
- Violation of the principle of least privilege.
- Modyfying URL,HTML-page and application state to bypass AC checks.
- Poorly or un-configured AC on API:s, allowing unauthorized POST,PUT&DELETE actions.
- Privilege elevation.
- Manipulation of metadata.
- Poorly configured CORS, allowing wrongfull actions through API's. 

**Prevention**
- Most of the time: deny by default.
- Implement AC mechanisms once, and reuse throughout.
- AC failure logs (put alerts in place).

>*Question*
>
> The article said, that AC is only effective in trusted server-side code.
> How would you implement a solution, that works also after an attacker gains access to the server, or if the attacker somehow manages to shut it down?


### A05:21 Security Misconfiguration

Causes for security vulnerabilites in applications.
- Having unnesessary features in use/installed.
- Too revealing/overly-informative error messages
- Not using or properly configuring latest security features.
- Outdated software and components.

**Prevention**
- Using a minimal platform, containing only the necessities.
- Automated secure environment setups.
- Using the same repeatable hardening process across environments, configured identically with different credentials.
- Application segmentation.

*Something to think about*
>
> How do you motivate/help people keep unique passwords across various platforms and enviroments.




### A06:21 Vulnerable and Outdated Components
> A broad category, that has a huge impact.

**Vulnerabilities arise from:**
- Not being aware of all the components versions in use.
- Using out of date and/or unsupported software.
- Not doing regular vulnerability scans.
- Not keeping up with the latest security news related to the components at work.
- Poorly secured component configurations.
- Not maintaining/updating/fixing regurarly.


**Prevention**
Take the previous section, turn it into the positive counterparts, and voila' 


*Thoughts*
>
> This is something that should be kept under tight reign.
> If you're using outdated, vulnerable & unsupported components and software, you will render most security mechanisms useless...




### A03:21 Injection
There is one main reason for this to be a major vulnerability. 

And that when data provided by user is not validated, filtered or sanitized.

There so many ways things that can go wrong from this inital point. 

Prevent against injections by cleaning up and checking user input, and adding query controls.





# WebGoat (A-B)

Latest version of webgoat can be found on github. 
![Screenshot 2025-02-06 at 17 20 06](https://github.com/user-attachments/assets/19c9e4f2-e2d5-4eb3-8b4d-8956450a34c1)

Confirm:
<img width="489" alt="Screenshot 2025-02-06 at 17 23 42" src="https://github.com/user-attachments/assets/45bf35e2-efe9-4c1e-900a-0083034235ef" />

I then started the program in the terminal.
<img width="472" alt="Screenshot 2025-02-06 at 17 25 32" src="https://github.com/user-attachments/assets/06cc829b-03e2-4e58-801a-4db619b68773" />

It initiated the program, and gave me the target to paste into a browser.
<img width="1023" alt="Screenshot 2025-02-06 at 17 25 57" src="https://github.com/user-attachments/assets/281897b2-95c8-4313-983c-472d9e15d0c6" />


The game was on.
<img width="1119" alt="Screenshot 2025-02-06 at 17 26 42" src="https://github.com/user-attachments/assets/d19977c2-8904-4f00-be5e-141ad25e6444" />


The General --> Developer tools, gave me a small introduction to HTML pages and javascript execution etc. 
<img width="1115" alt="Screenshot 2025-02-06 at 17 29 56" src="https://github.com/user-attachments/assets/4767dc52-917e-4b52-b504-400a61531f59" />

Next, it was time to open up the console and do a little test run, by running a javascript console log:
<img width="1122" alt="Screenshot 2025-02-06 at 17 35 33" src="https://github.com/user-attachments/assets/12d35124-9bad-465b-bdf9-8bd0afc7c742" />

Now was time for the first actual task. 
The idea was to start a javascript program by making a function call in the console.
I succesfully ran the function, got a number, pasted it in the box, and got my first task succesfully completed:
<img width="1123" alt="Screenshot 2025-02-06 at 17 42 07" src="https://github.com/user-attachments/assets/710aab2a-e612-4b0e-b3be-a69fc8c63cd4" />


Nextup there was some briefing again, talking about the devtools and how you can view different material. 

The next completable task was to generate HTTP traffic, locate the request, and copy the number in the data.
This was also a huge success!
<img width="1119" alt="Screenshot 2025-02-06 at 17 53 17" src="https://github.com/user-attachments/assets/cdcf615f-06d0-4be0-a4de-d6532c8870f1" />


*Final thoughts*
> WebGoat seems absolutely legit.
>
> I'm definitively going to use it in the future.
>
> I had some time to browse through the site, and it seems like you should have same prior knowledge & experience before cracking on with the game.
 >As they only explain what technique to use and what vulnerabilites to exploit, and not how & why. It would be good to know the tecniques at hand!




 # System update (C) 
- sudo apt update && sudo apt upgrade -y. Will do the trick!
- Nothing special here.



  

# SQLZOO (D)
### Part 1
>
> Starting off light
>

Pretty easy, pretty nice. Some basic SQL syntax.
<img width="367" alt="sqlzoo" src="https://github.com/user-attachments/assets/3f2eebd2-8b00-4a88-9026-0d6ca1fa82fb" />

![Screenshot 2025-02-06 at 18 17 19](https://github.com/user-attachments/assets/43db5e80-8e60-4f14-b9c3-3c31d20a979d)


### Part 2
>
>Diving deeper
>

After the initial familiarization, it was time to start combing through the database table. The first task was to pick countries with a population above 2 million, and display the names.
![Screenshot 2025-02-06 at 18 14 48](https://github.com/user-attachments/assets/9186fb35-ee78-4a8c-a3e0-12652a036c46)


This one was a bit more of a technical query. One had to select the same same condition as last, but this time divide the gpd with the population and show the results. 
Here we go:
![Screenshot 2025-02-06 at 18 19 26](https://github.com/user-attachments/assets/7266a2cc-8eab-4874-b0f8-e24dc8085739)


*Thoughts*
>
> The SQL and databases seems intuitive/easy enough to learn the basics off, which i'm definitively going to do. It is a good knowledge to have.
>
> Besides, you can't really dive deeper into the IT-security-realm, if you don't know how databases function (atleast on a basic level). They play a crucial role in our interconnected world.




# PortSwigger (E)
I made an account into PortSwigger and selected the SQL Injection course/module as my first learn in this environment. 
After going through the basics, I was navigated to continue on to my first lab. 

![Screenshot 2025-02-07 at 11 15 56](https://github.com/user-attachments/assets/9dfa2dbc-5565-4bce-b49e-63066775b8e0)


The lab took me to a mock shopping site
![Screenshot 2025-02-07 at 11 19 22](https://github.com/user-attachments/assets/1d10e566-5500-4943-a64e-ab78e941aae9)


I simply pressed on category: gifts. It gave me the following URL
![Screenshot 2025-02-07 at 11 25 11](https://github.com/user-attachments/assets/fb59a98f-a673-4053-b333-aa131ff356ea)


By first typing a simple ', i got en error message of: internal server error. 
This indicated that the site was vulnerable to SQLinjection, and that I could modify the url to perform my own query.
Which is exactly what i did

![Screenshot 2025-02-07 at 11 25 36](https://github.com/user-attachments/assets/733a1109-3ca2-4219-b824-ae4289e6cc30)

The Gifts'+OR+1=1-- injection, gives me all the hidden products in all categories, as 1 will always equal 1, so the OR clause is true. 
The rest of the query is then commented out with the "--".


### Confirmation
![Screenshot 2025-02-07 at 11 23 14](https://github.com/user-attachments/assets/292d3470-cb5f-4429-b30b-8403aef2d61e)



*Thoughts*
>
> I learned alot from just a quick & simple introduction and one small lab.
> This tells me i would be a fool not diving deeper into PortSwigger. I'm going to stay active on there, and dvelve into more subjects, as i'm expanding my horizons.
>
> I especially enjoyed the hands on learning style. You go through some theory, and then get to put the theory into practice.
>
> **About the topic:**
> - SQL injections are very intriguing. How one can perform own queries and manipulate the database, just by understanding the underlying concepts.
> - Also gave me an insight into how crucial it is, not to let raw user data interact with the database. Or any other underlying components for that matter.


![Screenshot 2025-02-05 at 21 12 02](https://github.com/user-attachments/assets/ce0f3dfb-a318-48b8-8544-9a5e1adae0bb)


### Lesson learned

Always sanitize the input! 



# Bonus (MN)


### WebGoat (SQL injection)

I started up my webgoat page as done before, and navigated to the SQL Injection module, there was some basic theory, and a few exercises.
<img width="1118" alt="Screenshot 2025-02-08 at 14 44 49" src="https://github.com/user-attachments/assets/7d2997e6-41ee-4637-8820-050dc7479431" />

<img width="852" alt="Screenshot 2025-02-08 at 14 48 59" src="https://github.com/user-attachments/assets/3a50c46f-d041-4315-8ddc-a5a176a2ffe5" />



After being able to aquire some data from the employee table, it was time to modify it. The assigment was to modify an employees department column. 
<img width="903" alt="Screenshot 2025-02-08 at 14 59 37" src="https://github.com/user-attachments/assets/fe2c4d8c-b4ac-4b91-a5d5-ebc1a7d55329" />


Nextup, we wanted to add a columnn of our own, this can be achieved easily by the following command: ALTER TABLE (*insert table*) ADD COLUMN (*insert column name and type*)

<img width="828" alt="Screenshot 2025-02-08 at 15 09 30" src="https://github.com/user-attachments/assets/0f64d16f-5af2-4542-b0d8-3433be74a9dc" />

Now that we knew how the basics of retreiving data and modifying it ( + the schema). Naturally we want to know how to modify access rights. That can be initiated with the command GRANT (pretty intuitive right?). Consecuently, if we wan't to remove a right from someone, intuitively we just start the query with "REVOKE".
<img width="816" alt="Screenshot 2025-02-08 at 15 13 25" src="https://github.com/user-attachments/assets/5e43330b-5ca9-4324-b149-ae8c350d2c05" />


In the next task, we knew the SQL query concatenates string, so by modifying it with lastname' or '1'='1 we can manipulate it
<img width="855" alt="Screenshot 2025-02-09 at 13 20 22" src="https://github.com/user-attachments/assets/2ab643db-be9d-49fa-a50b-c0762c0f8234" />


Here, the query concatenates dynamically the same way as the last one, but this time with numbers. So it is bypassed by simply typing 1 OR 1=1 without the apostrophes, in the latter box.
<img width="824" alt="Screenshot 2025-02-09 at 13 17 27" src="https://github.com/user-attachments/assets/eebadca4-3572-42e2-a1db-c8abaaf021f2" />

*Compromising the Confidentiality*

By knowing the query which was to be performed, we could simply type in whatevername' OR 1=1 --. This way we get a boolean value that gives us all entries, and comment out the rest of the query.
<img width="840" alt="Screenshot 2025-02-09 at 13 30 22" src="https://github.com/user-attachments/assets/7fff551f-6cd0-419d-aac9-4911e783fb57" />


*Compromising the Integrity*

After we just got the info on how much everyone makes, now we obviously want to change our own salary. 

I used the following command in the name field:

**Smith'; UPDATE employees SET salary = 90000 WHERE auth_tan = '3SL99A'; --** and then just a random value in the next field.
- The < Smith'; > succesfully check the name against the database, and then end the query so we can start a new one.
- Now we can modify entries with the UPDATE command, and specifying what we want to modify.
- The < '3SL99A'; -- > locates our own entry, modifies the salary, ends the command and comments out everything else from being executed after that. 
<img width="824" alt="Screenshot 2025-02-09 at 13 53 57" src="https://github.com/user-attachments/assets/dcd37d1c-e6c9-400e-b1aa-863ce88251db" />

*Compromising the Availability*

We wanted to delete any traces of our actions, by simply deleting the access log table. This was achieved be the following command.

**somethingrandom' DROP TABLE access_log'; --**

After the apostrophe we sent the signal do delete the table, and then signaled to end the command and comment out any remains of the original query.

<img width="1116" alt="Screenshot 2025-02-09 at 14 20 41" src="https://github.com/user-attachments/assets/49b74d84-2eeb-48c9-a91f-9dcaf669964c" />

And here we have it folks. That was the end to a decent introduction into SQL injections. Pretty fun, pretty nice & pretty informative.

### PortSWigger

I did the next lab relating to SQL injections on PortSwigger aswell. The lab took us to the same mock site as before, and the idea was to log in without a password. 
By assuming there is still a default admin user in place, we can use that to our advantage. 
![Screenshot 2025-02-07 at 12 11 44](https://github.com/user-attachments/assets/08b92362-b996-477c-8830-a88bebcfa6a0)


By typing in the username field: Administrator'--, and then just typing whatever into the password field (doesn't matter), we can bypass the password. 
Here is how it works: The apostrophe + --, comments out the rest of the query again, so the SQL query doesn't check for the password, and if the username match, it let's us in. 

![Screenshot 2025-02-07 at 12 13 57](https://github.com/user-attachments/assets/5494cea2-272e-470b-ae59-a29d5f66c039)

Boom goees the dynamite. And we're in!
