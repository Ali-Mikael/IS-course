# 7 Things you should know about tor (X)
> <https://www.eff.org/deeplinks/2014/07/7-things-you-should-know-about-tor> - Cooper Quintin (2014)

1. As long as your network traffic isn't being monitored, your browser is up to date and you don't have any misconfigurations, tor works, meaning it's completely anonymous.
2. It's not only for people hiding from the law. Various people use it to protect free speach, privacy,  anonymity and secure communications.
3. Tor is open software and has no backdoors.
4. At the time of writing the article, no one in the US has been prosecuted for running a Tor relay.
5. Tor is easy and simple to use!
6. Tor might be slower than a regular Internet connection, but not as slow as some might think. Developers are working hard to make Tor faster.
7. Tor is some of the strongest anonymity software that exists, however, it's not perfect. Misusage & configurations, as well as outdated software are main reasons for Tor to fail. 

<br>


# Hiding behind the keyboard (X)
> <https://learning.oreilly.com/library/view/hiding-behind-the/9780128033524/XHTML/B9780128033401000021/B9780128033401000021.xhtml#s0010>
> Brett Shavers & John Bair (2016)

## Chapter 2 
**Introduction**
- Tor: The Onion Router browser. Modified from the Firefox browser.
- With modifications, tor hides it's users IP-address, making anonomoys interaction on the internet possible for anyone with an internet connection and said Tor browser.
- While there are other means of hiding you IP-address, Tor's ingenuity stems from it's easy of use and not needing any technical skills to fully operate it. <br>


**History and Intended Use of The onion Router**
- Allthough Tor was initially developed by the US government in 2002, it is not controlled or operated by them present-day. 
- Usage: Unrestricted anonymous internet communication, allowing free speach, accessing of government blocked sites, whistleblowing and security over the internet, to name a few. <br>

**How The Onion router Works**
- Tor routes users Internet traffic through random relays on the internet.
- The data in transit is layered with elliptic curve cryptographty, which is (at the time of writing the chapter) immune to brute-force attacks.
- The data goes through 3 logical steps when passed through different relays.
  - Entry -> Middle -> Exit.
- Every relay uncovers a layer of cryptography, and sends it forward. The last step, from exit relay to destination, being unencrypted.
  - This process is kind of like peeling layers of an onion, hence the name: The **Onion** Router
- Out of the whole path, the exit relays knows only the previous relay. The route being chosen at random, and changed every ~10 minutes, making it almost impossible to track. <br>

**Tracking Criminals Using Tor**
- "*The most common goal of any Internet-related investigation is obtaining the true IP address*".
- The strong anonymity and security that comes with Tor, makes it an extremely difficult, time consuming and resource intensive task tracking down criminals.
- The biggest weakness in the browser is: *the user.*
- Most investigations rely solely on the user making a mistake, and thus giving away his true IP-address.
- 2 quick examples:
  - A misconfigured browser/allowed plugins, could result in opening up a link which would have the permission to execute code, which in turn could lead exposing your true IP-address.
  - Using the Tor browser in a company/school network. Even though the IT-admin wouldn't see the contents of the communication, he could she that there was in fact Tor related internet activity. This commbined with some fraudulent/criminal activity performed in a certain time-frame (matching the Tor activity in the network), could lead to a suspect initially being caught, and later broken under questioning. 
- But the point stands. It's not reasonable to start cracking the Tor browser, rather you rely on it's users making mistakes, in order to catch the criminals.


<br> <br> <br>




# Installing the dark browser (A)
> <https://terokarvinen.com/information-security/> <br>

- Started off my firing up the ol reliable kaliVM, and locating the Tor browser download page. 
- <img width="1116" alt="Screenshot 2025-03-07 at 15 43 43" src="https://github.com/user-attachments/assets/0a85dd39-6050-445b-9f33-4c0651339618" />

`tar -xf tor-browser`




# Browsing in the dark
