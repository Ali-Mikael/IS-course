# Owasp 10

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





#WebGoat

I downloaded WebGoat on my vm, from github. 
I




SQLzoo





