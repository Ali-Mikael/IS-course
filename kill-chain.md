# Intelligence-driven Computer Network Defence
> The Lockheed Martin Corporation backed paper on cyber kill chain, id an intriguing piece of paper, that provides a fundamental framework for APT (Advanced Persistent Threat) analysis and mitigation. 

## Down below i'm going to dissect what i read, using summarizations and bullet points, and also provide some of my own insight
Let's dive right in!

### What is an APT 
> APT = " A systematic process to target and engage an adversary to create desired effects"
#### By whom? 
> Well resourced & trained adversaries (threat-actors), that conduct multi-year intrusion campaigns.
> The US military doctrine of kill chain = find, fix, track, target, engage & asses.
> The new cybsec kill chain model, specifically for intrusions, presented in the paper = reconnaisance, weaponization, delivery, explotation, installation, C2 & actions on objectives

## Conventional CND has focused on tehcnologies reducing the risk of automated worms & viruses
>This simply doesn't cut it in APT's, as they are manually operated, focused intrusions that are driven by patience and calculated moves.
>The old model makes 2 flawed assumptions: Response after compromise, and said compromise resulted of a fixable flaw


## Indicator - the fundamental element of the kill chain model
### Definiton - Any piece of information that objectively describes an intrusion
### 3 types of indicators:
> *Atomic* - Cannot be broken down into smaller parts without losing their meaning in the context of intrusion
> *Computed* - Derived from data involved in an incident
> *Behavioral* - Collections of computed and atomic indicators

 ## Key notes - defending APT's
 > In order for defenders to use the persistence of adversarys against them, one must completely understand an intrusion, and use intelligence on the used tools and infrastructure
#### Synthesis:
> Synthesis of unsuccesful intrusions is equally as important as thorough analysis of succesful compromise. 
> Defenders must collect as much data as possible from a mitigated intrusion attempt, in order to reconstruct what could've actualised in a later phase. 
> The knowledge of what could've happened, helps to defend future intrusions, should they go past the current mitigation & detection. 
