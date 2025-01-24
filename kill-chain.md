# Intelligence-driven Computer Network Defence
The Lockheed Martin Corporation backed paper on cyber kill chain, is an intriguing piece of paper, that provides a fundamental framework for APT (Advanced Persistent Threat) and mitigation. 

## Down below i'm going to dissect what i read, using summarizations and bullet points, and also provide some of my own insight
Let's dive right in!

### What is an APT?
APT = " A systematic process to target and engage an adversary to create desired effects"
### By whom? 
Well resourced & trained adversaries (threat-actors), that conduct multi-year intrusion campaigns.
### The "Kill chain"
The US military doctrine of kill chain = find, fix, track, target, engage & asses.

**The new cybsec kill chain model, specifically for intrusions, presented in the paper:**
- *Reconnaisance*

- *Weaponization*

- *Delivery*

- *Explotation*

- *Installation*

- *C2 (Command & Control)*

- *Actions on objectives*

>**Insighs:**
>
> - This gives a rather clear & linear framework on the adversary kill chain.
> - The model is excellent for it's simplicity, and readability, and gives you tools in mapping the actions and phases of an adversary.
> - Furthermore, it helps you in analyzing the actions more thoroughly, which in turn gives you an advantage going into future intrusion attempts.
> - In my opinion this should be used in conjunction with other frameworks rather than as a standalone.
> - Like the writer stated, "Responses to APT intrusions require evolution of analysis, process and technology", so should this framework also evolve.


### Conventional CND (Computer Network Defence)
Has focused on tehcnologies reducing the risk of automated worms & viruses.
- The old model makes 2 flawed assumptions: Response should happen after compromise, and said compromise being the result of a fixable flaw.
- This simply doesn't cut it in defending APT's, as they are calculated, manually operated, focused intrusions, that are executed with patience and drive.


### APT kill chain analysis
The fundamental intelligence in this model, are the *indicators*.

An indicator in this context: A *fundamental element* of the kill chain model.

Definiton - **Any piece of information that objectively describes an intrusion**.

**There are 3 types of indicators:**
- *Atomic* - Cannot be broken down into smaller parts without losing their meaning in the context of intrusion.
- *Computed* - Derived from data involved in an incident.
- *Behavioral* - Collections of computed and atomic indicators.


>**Insights**
>
> - The indicators give concrete examples, on how intelligence is used in this intelligence-driven CND model.
> - With the use of indicators, one can gather crucial insight into intrusion methods and tactics, compare them together, to build a strond defence against future intrustion attempts.


### Defending APT's
 > In order for defenders to use the persistence of adversarys against them, one must completely understand an intrusion, and use intelligence on the used tools and infrastructure.

**Synthesis:**
- Synthesis of unsuccesful intrusions is equally as important as thorough analysis of succesful compromise.

- Defenders must collect as much data as possible from a mitigated intrusion attempt, in order to reconstruct what could've actualised in a later phase. This could lead to
  the discovery of new exploits or backdoors for example.

- The knowledge of what could've happened, helps to defend future intrusions, should they go past the current mitigation & detection.

A crucial part in defending against APT's is understanging the adversary.
- Patterns & behaviour
- Tactics, Techniques & Procedure
- Intent
  > Learn the objective of the adversary.
  >
  > This can be achieved for example, by closely examining any exfiltrated data.

### Strategy
- Analyzing multiple intrusion kill chains over time, will identify commonalities and overlapping indicators.
- Intrusion campaigns might have varying degrees of similarities, but with thorough analysis, it is possible to illustrate key indicators.

>**Insights**
>
> - Building a holistic, informed and consistent strategy is crucial for defending APT's.
>
> - With the use of key indicators, understanding adversary objectives and knowledge of technologies & infrastructure, one has the building blocks to build a resiliant strategy against APT's.
