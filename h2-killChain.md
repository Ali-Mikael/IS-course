# Intelligence-driven Computer Network Defence
>
The Lockheed Martin Corporation backed paper "Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains", is an intriguing piece of paper, that provides a comprehensive framework for APT (Advanced Persistent Threat) and mitigation.
>

## Down below i'm going to dissect what i read, using summarizations and bullet points, and also provide some of my own insight
Let's dive right in!


### What is an APT?
- APT (Advanced Persistent Threat) = " A systematic process to target and engage an adversary to create desired effects"
### By whom? 
- Well resourced & trained adversaries (threat-actors), that conduct multi-year intrusion campaigns.
### The "Kill chain"
- The US military doctrine of kill chain = find, fix, track, target, engage & asses.

**The presented cybsec kill chain model, specifically for intrusions:**
- *Reconnaisance*

- *Weaponization*

- *Delivery*

- *Explotation*

- *Installation*

- *C2 (Command & Control)*

- *Actions on objectives*

>**Insighs:**
>
> - The proposed framework gives a rather clear & linear insight on the phases of an APT. It's excellent for it's simplicity and readability.
> - The framwork gives you tools, in mapping the actions and phases of an threat-actor, to help you better undestand them, in order to mitigate them.
> - In my opinion this should be used in conjunction with other frameworks rather than as a standalone.
> - Like the writer stated, "Responses to APT intrusions require evolution of analysis, process and technology", so should this framework also evolve.


### Conventional CND (Computer Network Defence)
- Conventional methods have focused on tehcnologies reducing the risk of threats, such as automated worms & viruses.
- The old model makes 2 flawed assumptions: Response should happen after compromise, and said compromise being the result of a fixable flaw.
- This simply doesn't cut it in defending against APT's, as they are calculated, manually operated, focused intrusions, that are executed with patience and tenacity.


### The "Intelligence", in intelligence-driven CND
- The fundamental intelligence in this model, is the *indicator*.
- An indicator in this context: A *fundamental element* of the kill chain model.
- Definiton - **Any piece of information that *objectively* describes an intrusion**.

**There are 3 types of indicators:**
- *Atomic* - Cannot be broken down into smaller parts without losing their meaning in the context of intrusion.
- *Computed* - Derived from data involved in an incident.
- *Behavioral* - Collections of computed and atomic indicators.


>**Insights**
>
> - The objectifing of intrusion tactics and processes, is a really neat way of better understanding the abstract model.
> - With the use of indicators, one can more easily compare past intrusion attempts side by side.


### Defending APT's
 > In order for defenders to use the persistence of adversarys against them, one must completely understand an intrusion, and use intelligence on the used tools and infrastructure.

**Synthesis:**
- Synthesis of unsuccesful intrusions, is equally as important as thorough analysis of succesful compromise.
- Defenders must collect as much data as possible from a mitigated intrusion attempt, in order to reconstruct what could've actualised in a later phase. This could lead to
  the discovery of new exploits or backdoors for example.
- The knowledge of what could've happened, helps to defend future intrusions, should they go past the current mitigation & detection.

**A crucial part in defending against APT's is understanging the adversary.**
- Patterns & behaviour
- Tactics, Techniques & Procedure
- Intent
  > - Learn the objective of the adversary.
  > - This can be achieved for example, by closely examining any exfiltrated data.

### Strategy
- Analyzing multiple intrusion kill chains over time, will identify commonalities and overlapping indicators.
- Intrusion campaigns might have varying degrees of similarities, but with thorough analysis, it is possible to illustrate key indicators.
- Key indicators will be an immense asset, in building a stronger & more resiliant defence strategy.

>**Finishing insights**
>
> - I understood that building a **holistic**, **analytic** and **resiliant** strategy is crucial, for defending against APT's. Also the fact, that the game of cyberattacks have evolved from 2D to 4D chess over time.
> - One should approach the APT's and adversarys from an analytical, open-minded and dynamic perspective, in order to be effective in mitigation efforts.
> - The intelligence-driven CND model gives a fundamental/comprehensive look into the world of cyberSecurity, for anyone interested. 
> - "Know thy enemy"




**Source**
> https://lockheedmartin.com/content/dam/lockheed-martin/rms/documents/cyber/LM-White-Paper-Intel-Driven-Defense.pdf
