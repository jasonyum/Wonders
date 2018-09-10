[Odds Ratio Link](https://jamanetwork.com/journals/jama/fullarticle/2686777?utm_source=twitter&utm_campaign=content-shareicons&utm_content=article_engagement&utm_medium=social&utm_term=080818#.W2sEndGl794.twitter)

# Odds Ratios - Current Best Practice and Use

> Odds ratios frequently are used to present strength of association between risk factors and outcomes in the clinical literature. Odds and odds ratios are related to the probability of a binary outcome (an outcome that is either present or absent, such as mortality). The odds are the ratio of the probability that an outcome occurs to the probability that the outcome does not occur. For example, suppose that the probability of mortality is 0.3 in a group of patients. This can be expressed as the odds of dying: 0.3/(1 − 0.3) = 0.43. When the probability is small, odds are virtually identical to the probability. For example, for a probability of 0.05, the odds are 0.05/(1 − 0.05) = 0.052. This similarity does not exist when the value of a probability is large.

- odds = P(outcome occurs) / P(outcome doesn't occur) 
- EX: mortality % is 0.3 in a group of patients. 
  - Then the probability of not dying is 0.7.
  - Hence, the odds ratio = 0.3/(1-.3) = 0.43. 
  - When the probability is small, the odds are virtually identical. 
    - Like probability of 0.05 of death then it's 0.05/(1-0.05) = 0.052.

> Probability and odds are different ways of expressing similar concepts. For example, when randomly selecting a card from a deck, the probability of selecting a spade is 13/52 = 25%. The odds of selecting a card with a spade are 25%/75% = 1:3. Clinicians usually are interested in knowing probabilities, whereas gamblers think in terms of odds. Odds are useful when wagering because they represent fair payouts. If one were to bet $1 on selecting a spade from a deck of cards, a payout of $3 is necessary to have an even chance of winning your money back. From the gambler’s perspective, a payout smaller than $3 is unfavorable and greater than $3 is favorable.

- Odds are useful when wagering because they represent fair payouts. 
- Relative risk ratio = ratio of two probabilities (not necessary from the same binary).

## Why Report Odds Ratios from Logistic Regressions? 

> Researchers often analyze a binary outcome using multivariable logistic regression. One potential limitation of logistic regression is that the results are not directly interpretable as either probabilities or relative risk ratios. However, the results from a logistic regression are converted easily into odds ratios because logistic regression estimates a parameter, known as the log odds, which is the natural logarithm of the odds ratio. For example, if a log odds estimated by logistic regression is 0.4 then the odds ratio can be derived by exponentiating the log odds (exp(0.4) = 1.5). It is the odds ratio that is usually reported in the medical literature. The odds ratio is always positive, although the estimated log odds can be positive or negative (log odds of −0.2 equals odds ratio of 0.82 = exp(−0.2)).

- Results from a logistic regression may not be directly interpretable as either probabilities or relative risk ratios. 
- Log odds = natural log of the odds ratio. 
- If log odds = 0.4 then the odds ratio = exp(0.4) = 1.5. (simple math) 


## What are the Limitations of Odds Ratios? 
- Odds ratios are often mistake for relative risk ratios. 
- Odds ratios tend to overestimate relative risk ratios, except for rare outcomes.

> Second, and less well known, the magnitude of the odds ratio from a logistic regression is scaled by an arbitrary factor (equal to the square root of the variance of the unexplained part of binary outcome). This arbitrary scaling factor changes when more or better explanatory variables are added to the logistic regression model because the added variables explain more of the total variation and reduce the unexplained variance. Therefore, adding more independent explanatory variables to the model will increase the odds ratio of the variable of interest (eg, treatment) due to dividing by a smaller scaling factor. In addition, the odds ratio also will change if the additional variables are not independent, but instead are correlated with the variable of interest; it is even possible for the odds ratio to decrease if the correlation is strong enough to outweigh the change due to the scaling factor.

- Adding more independent explanatory variables to the model will increase the odds ratio! 
- This happens because you're dividing by a smaller scaling factor.
- The scaling factor is the square root of the variance of the unexplained part of the binary outcome.

