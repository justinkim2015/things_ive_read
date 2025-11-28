# LLM Output Configuration

After choosing a model you will have to set your models configuration.  The following are common settings:

## Output Length
This is the number of tokens to generate in a response.  The more tokens used generally equates to slower response times and higher costs.  By reducing this setting, the LLM doesn't become more succinct, rather it just stops predicting future tokens and cuts off.

Output length restriction is important for some LLM prompting techniques like ReAct, where the LLM will keep emitting useless tokens after the response you want.

## Sampling Controls

LLMs predict probabilities for what the next token could be (not just one), with each token in the LLM's vocabulary getting a probability.  Those token probabilities will then be sampled to determine what the next produced token will be.  The following settings determine how these predicted token possibilities are processed to a single token.

### Temperature
This controls the degree of randomness in a token selection.  The lower the temperature, the more deterministic the LLM response will be.  A higher temperature will produce more random and surprising results.

### Top-K and Top-P
Top-K and Top-P (AKA nucleus sampling) are two sampling settings used to restrict the predicted next token to come from tokens with the top predicted probabilities.  These settings will also control the randomness and diversity of generated text.

#### Top-K
This selects the top K most likely tokens from the model's predicted distribution.  The higher the top-K, the more creative and varied the model's output will be, where the lower top-K, the more factual the models output will be.

#### Top-P
This sampling selects the top tokens whose cumulative probability does not exceed a certain value (P).  Values for P range from 0 (factual) to 1 (all the tokens in the LLM's vocabulary)

## Putting it all together
When combining these four configurations together, it will work in this order.

1. All the tokens that meet the top-K and top-P criteria are candidates for the next predicted token.
2. Temperature is applied to the sample from the tokens that passed the criteria in step 1.

With extreme settings some configuration settings can cancel the other out:
- With a temperature of 0, top-K and top-P become irrelevant.  You will always pick the most probable next token, therefore the filtering done by top-k and top-p won't matter.
- With a very high temperature (1+), temperature becomes irrelevant, it will randomly pick a token that was not filtered by the top-k and top-p settings.
- If top-k is 1, temperature and top-p are irrelevant, because only 1 token will be selected, therefore it will always be the next created token.
- If top-p is 0, temperature and top-k are irrelevant, because most likely only the most probably token will be selected by the top-p criteria and it will be the next outputted token.

> A suggested starting point is: temperature = .2, top-P = .95, top-k = 30.  This will give you coherent but creative results. 