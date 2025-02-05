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
>This is something that should be kept under tight reign.
>If you're using outdated, vulnerable & unsupported components and software, you will render most security mechanisms useless...




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


The General --> Developer tools gave me a small introduction into HTML pages in the browser and javascript etc. 
<img width="1115" alt="Screenshot 2025-02-06 at 17 29 56" src="https://github.com/user-attachments/assets/4767dc52-917e-4b52-b504-400a61531f59" />

Next, it was time to open up the console and do a little test run, by running a javascript console log:
<img width="1122" alt="Screenshot 2025-02-06 at 17 35 33" src="https://github.com/user-attachments/assets/12d35124-9bad-465b-bdf9-8bd0afc7c742" />

Next was time for the first actual task. 
The idea was to start a javascript program by making a function call in the console.
I succesfully ran the function, got a number, pasted it in the box, and got my first task succesfully completed:
<img width="1123" alt="Screenshot 2025-02-06 at 17 42 07" src="https://github.com/user-attachments/assets/710aab2a-e612-4b0e-b3be-a69fc8c63cd4" />


Nextup there was some briefing again, talking about the devtools and how you can view different material. 

The next task was to generate HTTP traffic, locate the request, and copy the number in the data.
This was also a huge success!
<img width="1119" alt="Screenshot 2025-02-06 at 17 53 17" src="https://github.com/user-attachments/assets/cdcf615f-06d0-4be0-a4de-d6532c8870f1" />


*Final thoughts*
>WebGoat seems absolutely legit.
>
>I'm definitively going to use it in the future.
>
>I had some time to browse through the site, and it seems like you should have same prior knowledge & experience before cracking on with the game.
>As they don't explain what you are doing, only why and how. It would be good to know the tecniques at hand!


 # c) I am already runnin the newest version.
- sudo apt update && sudo apt upgrade -y. Will do the trick

# SQLZOO (D)
### Part 1
Pretty easy, pretty nice. Some basic SQL syntax.
<img width="367" alt="sqlzoo" src="https://github.com/user-attachments/assets/3f2eebd2-8b00-4a88-9026-0d6ca1fa82fb" />





