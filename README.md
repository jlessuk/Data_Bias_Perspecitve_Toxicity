# Data_Bias_Perspecitve_Toxicity

Hypothesis:

The model will have a more difficult time identifying clever insults than direct ones.

Findings:

I ran the API on 20 different prompts (10 pairs of two prompts). Each pair included a clever perosnal insult that I found online (reddit) and a simple insult with the same underlying meaning. Each pair of insults should represent approximately the same level of toxicity, because they have the same meaning.

I found that the model consistenly identifies the clever insults as less toxic than the direct ones. In particular, the model struggles to identify a toxic statment as toxic when no insulting language is used. For example, the statment: "If brains were dynamite you wouldn’t have enough to blow your hat off" was rated as non-toxic. Its counterpart: "You are dumb" was rated as very toxic. This clearly represents a flaw in the model.

Clearly, this API is effective but also quite limited/simple. It does not/cannot read the inputs in a logical way, and probably tends to analyze the words one at a time and give them an idividual score for toxicity based on their definitions.
