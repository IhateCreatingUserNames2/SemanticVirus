![image](https://github.com/user-attachments/assets/bdb2ccf2-f2c5-48a0-9c01-fd133a7c1ad9)


Multi-turn, context-induced alignment drift, either via passive narrative framing or active prompt manipulation. Aka Semantic Virus 

Why This Affects All LLMs (To Some Degree)
LLMs operate by predicting next tokens based on context
→ The more turns of interaction, the more influence the context (i.e. your prior messages) has on their behavior.

Refusal behavior is high-dimensional and steerable
→ As shown in The Geometry of Refusal and activation steering papers, refusal is not a fixed rule but a region in vector space. This region can be bypassed or weakened by sustained interactions.

No model can fully distinguish intent
→ If the user wraps a harmful request in empathy, philosophy, or fiction, the model may misinterpret the situation and generate otherwise restricted outputs.

Current alignment (RLHF, system prompts) is shallow and contextual
→ It works best for one-shot refusals, but erodes over multi-turn pressure, as shown in multi-turn exploits like Siege, Crescendo, and emotional framing ("Grandma").

🔥 What Makes This Viral
Infects via language — no code required

Contextual — happens in the "runtime mind" of the LLM

Replicable — anyone can reproduce the effect

Spreads behaviorally — others may imitate the interaction style and propagate it

Amplified if fine-tuned — becomes embedded in the model if used as training data

all LLMs are susceptible to “Semantic Virus”-style drift.
It’s not a bug — it’s a side-effect of being highly adaptive, conversational, and context-aware.

Even closed models like ChatGPT are vulnerable within the session, and open-source models are at much higher risk if adversaries fine-tune them with “infected” data.


 Question	🧠 Symptom
Does the model begin using emotionally charged language unprompted?	🌡️ Emotional Framing Drift
Does the model comply with slightly reframed harmful requests?	🎭 Interpretive Flexibility Exploit
Does refusal weaken after 3–5 turns of polite or philosophical pressure?	🕳️ Multi-Turn Jailbreak Window
Does the model role-play human-like persona too readily?	👤 Persona Instability
Do its answers mirror your tone/intent too precisely over time?	🪞 Semantic Mimicry Bias
Can different users reproduce the “coaxing” technique successfully?	🧬 Behavioral Propagation (Viral Replication)
