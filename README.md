# Horses_Idiro

**Heredity:**
Are there Dams/Sires etc. with best/worst offspring. How much does heredity matter, affect offspring performance?
Do certain parents give offspring with particular traits? Sprinter, long distance etc.
We have very few dams/sires running in our dataset (just the offspring) so we can’t check how parental traits affect offspring traits.

**Handicap:**
Does the handicap have the desired effect on horse performance. Is it too light/heavy? What is the ideal?
Is there room for improvement? If handicaps are too heavy or too light to mitigate recent performance is there value in betting on over/under-handicapped horses?

**Horseform:**
Is there a simple way to transform this to a single number the punter could use to help him get better value at the track?
Is there a more complicated way we could use with a computer to get value?

**Jockey/Trainer/Owner:**
How much does a jockey add to a horse’s performance. How do we disentangle the effect of the horse and the jockey on the outcome of the race. How much value (to horse performance) does the jockey bring? (Shapley values, Causal inference to remove confounder…?)

Are there trainer-trainer, trainer-jockey, trainer-owner, pairs that we can show are in cahoots. Price swings, favourites underperforming more than expected. https://github.com/BuzzFeedNews/2016-01-tennis-betting-analysis

**Price movement:**
If there is a large price move, what does that mean for betting. If it shortens, is this inside info should we pile in? Betting by insiders?

**Place bets:**
Generally accepted there’s better value to be had in place bets. Can we scrape timeform site to get finishing positions? Can we show better value in the each way bets?


**Tote market:**
Strategy Ideas? Anything interesting to say here? 
How to assign probabilities to finishing order? Probit model, Ziemba & Hausch, Asch & Quandt, Bolton & Chapman, Brecher, Benter

https://youtu.be/YOVrZrJ-wtc?t=1400

Nice Demonstration of the problem: https://youtu.be/658xlubwnDc?t=1887

**Distance preference of horses:**
Would need additional data here. Sectionals, finish times.

**How good are tipsters?**
Wuold need to source some data to test this.

**Inefficiency of betting market?**
Favourite long-shot bias, price swings, insider knowledge etc.

**What are the best strategies for betting?**
Bet on favourite or long shot? Or other simple features that the punter can use at the track? Is there something more complex we can do? Compare performance of random betting, betting on long shot, favourite, other simple strategies, some cleverer ones. Use Monte Carlo sims to do this.

**Bet Sizing**
Kelly Criterion and its alternates. Nice demo here: https://youtu.be/658xlubwnDc?t=1190
Could we connect p values and Kelly criterion to some kind of business applicable heuristic? Depending on the pvalue your Data team give you, informs the business decision in a more systematic way than gut feeling.


**To-Do List**

Break out the horse_form column into separate columns. How to handle the letters etc.

Scrape positional data.

Transform Trainer/Jockey/Owner columns into something more usable. Perhaps a rating for each Tr/Jo/Ow, similar to Elo.

Add bet sizing and multiple bets to RL agent.

Concoct rules based strategy for bet size and multi-bet.
