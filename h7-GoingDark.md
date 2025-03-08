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
> <https://learning.oreilly.com/library/view/hiding-behind-the/9780128033524/XHTML/B9780128033401000021/B9780128033401000021.xhtml#s0010> <br>
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
  - A misconfigured browser/allowed plugins = could result in opening up a link which would have the permission to execute code, which in turn would send information of your system to the creator, and could lead to exposing your true IP-address.
  - Using the Tor browser in a company/school network = Even though the IT-admin wouldn't see the contents of the communication, he could she that there was in fact Tor related internet activity. This commbined with some fraudulent/criminal activity performed in a certain time-frame (matching the Tor activity in the network), could lead to a suspect initially being caught, and later broken under questioning. 
- But the point stands. It's not reasonable to start cracking the Tor browser, rather you rely on it's users making mistakes, in order to catch the criminals.


<br> <br> <br>




# Installing the dark browser (A)
> Reference <br>
> <https://terokarvinen.com/information-security/> <br>

I navigated to the Torproject website <https://www.torproject.org/download/>, and downloaded the Tor browser.
- <img width="433" alt="Screenshot 2025-03-07 at 16 18 02" src="https://github.com/user-attachments/assets/dd142d70-46d3-4a77-a65d-0e17b106a454" /> <br>

After the installation was complete, I opened up the browser and established a secure connection.
- <img width="1387" alt="Screenshot 2025-03-07 at 16 19 05" src="https://github.com/user-attachments/assets/a695beef-68ba-496a-91ff-0ad271ce6c58" /> <br>

I then opened up DuckDuckGo .onion version, and was ready to start exploring! 
- <img width="1393" alt="Screenshot 2025-03-07 at 16 35 55" src="https://github.com/user-attachments/assets/d9f47f81-5b6e-4ee5-94e5-bedc103129f6" /> <br>

Some info on .onion, straight from the onion. 
- <img width="1349" alt="Screenshot 2025-03-07 at 16 26 16" src="https://github.com/user-attachments/assets/3f64bd0d-19e0-4559-99ef-7c3df06ef6ec" />

<br> <br> 

# Browsing in the dark
I managed to find an off brand Hidden-Wiki site, with some useful .onion links. 
- <img width="815" alt="Screenshot 2025-03-07 at 16 39 38" src="https://github.com/user-attachments/assets/513ae307-5386-468c-ba76-3200b3e42858" />
-<img width="558" alt="Screenshot 2025-03-07 at 16 39 51" src="https://github.com/user-attachments/assets/48572214-1793-4640-b040-f26d4fe85e12" />

- <br>
### DREAD
I navigated to the first link i saw, which was a chat forum called **Dread**.
- <img width="1129" alt="Screenshot 2025-03-07 at 16 40 54" src="https://github.com/user-attachments/assets/b0591ed6-8198-45fb-8fe4-afb330439547" />
- There was some pretty hefty stuff on the forum i'm not going to lie.
- First off I encountered some of the basics like drugs, weapons & violence.
- Ofcourse there were alot of people trying to scam others.
- Then I came accross interesting viewpoints on how to smuggle drugs and dispose of bodies, you know the usual stuff. For my own safety I won't be posting any more screenshots on here, just take my word for it!
<br>

### Blow the whistle
And then naturally, straight under the illegal stuff, you would have a section for reading about it on the news and reporting it anonymously to the authorities. 😂
- <img width="523" alt="Screenshot 2025-03-07 at 16 47 33" src="https://github.com/user-attachments/assets/52205270-ac41-43f2-b43e-c5a935a3f71c" />
- The links for the news outlets were an example of how some people might ingest news, as their home country have oppressing regimes which don't allow them to browse the internet freely. (I'm not going to comment how "free speech"/"free thinking" the likes of BBC are but whatever...)
- Here you could find the official .onion site for the CIA.
- <img width="1395" alt="Screenshot 2025-03-08 at 15 00 51" src="https://github.com/user-attachments/assets/5e4f0dcd-5a2a-432c-8d35-7527c3d1f3c5" />


<br>

### The OG Hidden-Wiki

I did some digging, until I found the orginial Hidden-Wiki page (atleast so I  think). 
- <img width="1393" alt="Screenshot 2025-03-07 at 16 51 06" src="https://github.com/user-attachments/assets/37ae2a33-7660-464c-a818-b41fa27095ee" />
- I browsed some links, seemed very interesting. The ones that caught my curiosity the most were the hacking related stuff, were people shared stories, knowledge and abilities amongst each other. 
- Also found this amusing **hackerforsale!** situtation going on.
  - <img width="981" alt="Screenshot 2025-03-08 at 14 55 05" src="https://github.com/user-attachments/assets/9b1622d2-6b53-47bf-a761-ed57fa68d903" />
- After browsing a while, I finally decided to join a live chat room to see how it looks like.
- <img width="1396" alt="Screenshot 2025-03-07 at 16 52 15" src="https://github.com/user-attachments/assets/470bf56b-a5e3-4424-9be9-a62bacc2ff80" />
- <img width="509" alt="Screenshot 2025-03-07 at 16 52 47" src="https://github.com/user-attachments/assets/18a12028-6d85-43ac-96e6-00ecee5b30e1" />
- <img width="1396" alt="Screenshot 2025-03-07 at 16 59 56" src="https://github.com/user-attachments/assets/375f4629-4fd8-454b-a701-9452997e9caf" />
- I didn't really interact there, as I was just lurking in the shadows and followed along. People were talking about guns, drugs & violence, you know the usual stuff. But then there was some banter here and there, some people trying to scam other, some trying to discuss crypto, some trying to sell pornography and suddenly it took a left turn and people started talking about their views on religion... Wild stuff! 😂
<br>
The onion web is a wild place, where everything goes. It can be a wonderfull tool, or a means to do evil. <br>
#### You decide!
  *Thread lightly,*
     *proceed at your own caution!*










