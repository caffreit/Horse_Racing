# Horses_Idiro

**Reading Material:**
https://drive.google.com/open?id=1-KaL1i8dwFU-pGJKVzasRCT5wxjGcXo7

https://www.pinnacle.com/en/betting-resources/archive

https://ideas.repec.org/s/bpj/jqsprt.html

http://ubplj.org/index.php/jpm/index

http://www.ubplj.org/index.php/jgbe/index


**Going:**
Needs to be scraped.
Horse Racing Ireland:https://www.goracing.ie/race-meetings/results/race-result/?date=2018-02-10&race=1335&venue=NS 
British Horse Racing Authority: https://www.britishhorseracing.com/racing/results/fixture-results/#!/2018/853


**Heredity:**
Are there Dams/Sires etc. with best/worst offspring. How much does heredity matter, affect offspring performance?
Do certain parents give offspring with particular traits? Sprinter, long distance etc.
We have very few dams/sires running in our dataset (just the offspring) so we can’t check how parental traits affect offspring traits.

https://www.theguardian.com/science/2014/jun/22/horse-breeding-genetics-thoroughbreds-racing-dna

**Handicap:**
Does the handicap have the desired effect on horse performance. Is it too light/heavy? What is the ideal?
Is there room for improvement? If handicaps are too heavy or too light to mitigate recent performance is there value in betting on over/under-handicapped horses?

**Horseform:**
Is there a simple way to transform this to a single number the punter could use to help him get better value at the track?
Is there a more complicated way we could use with a computer to get value?

**Jockey/Trainer/Owner:**
How much does a jockey add to a horse’s performance. How do we disentangle the effect of the horse and the jockey on the outcome of the race. How much value (to horse performance) does the jockey bring? (Shapley values, Causal inference to remove confounder…?)
http://bayes.cs.ucla.edu/home.htm

Are there trainer-trainer, trainer-jockey, trainer-owner, pairs that we can show are in cahoots. Price swings, favourites underperforming more than expected. https://github.com/BuzzFeedNews/2016-01-tennis-betting-analysis

**Price movement:**
If there is a large price move, what does that mean for betting. If it shortens, is this inside info should we pile in? Betting by insiders?

https://historicdata.betfair.com/#/help

https://historicdata.betfair.com/#/home

**Place bets:**
Generally accepted there’s better value to be had in place bets. Can we scrape timeform site to get finishing positions? Can we show better value in the each way bets?

https://www.timeform.com/horse-racing/shop/sectional-times has finish positions

https://www.timeform.com/commercial/products/api just has timeform rating etc.


**Tote market:**
Strategy Ideas? Exotic Bets (Exacta, Trifecta, Quinella) tend to have better value. I think due to misestimation of the more complicated set of outcomes. Or the cumulative effect of misestimation of odds.
How to assign probabilities to finishing order? Probit model, Ziemba & Hausch, Asch & Quandt, Bolton & Chapman, Brecher, Benter

https://youtu.be/YOVrZrJ-wtc?t=1400

Probability distribution of finish times/positions, sample at random for each horse building up a frequency/probability distribution of finishing positions.

Nice Demonstration of the problem: https://youtu.be/658xlubwnDc?t=1887

**Distance preference of horses:**
Would need additional data here. Sectionals, finish times.

https://www.timeform.com/horse-racing/shop/sectional-times

**How good are tipsters?**
Wuold need to source some data to test this.
https://www.tippingsports.com/betting-tips/tips

https://www.kaggle.com/gunner38/horseracing

**Inefficiency of betting market?**
Favourite long-shot bias, price swings, insider knowledge etc.

**What are the best strategies for betting?**
Bet on favourite or long shot? Or other simple features that the punter can use at the track? Is there something more complex we can do? Compare performance of random betting, betting on long shot, favourite, other simple strategies, some cleverer ones. Use Monte Carlo sims to do this. Risk of ruin, random walk. How best to allocate bet over multiple favourable bets? MathSport pg 219

**Bet Sizing**
Kelly Criterion and its alternates. Nice demo here: https://youtu.be/658xlubwnDc?t=1190
Could we connect p values and Kelly criterion to some kind of business applicable heuristic? Depending on the pvalue your Data team give you, informs the business decision in a more systematic way than gut feeling.


**To-Do List**

~~Break out the horse_form column into separate columns. How to handle the letters etc.~~

Scrape/Buy positional data.

Transform Trainer/Jockey/Owner columns into something more usable. Perhaps a rating for each Tr/Jo/Ow, similar to Elo.

Add bet sizing and multiple bets to Reinforcement Learning agent.

Concoct rules based strategy for bet size and multi-bet.

**Features:**

~~Induced Odds (from BackPrice)~~

~~Induced Odds (correct for OverRound & Fav-LongShot Bias)~~

~~Capture large change in Price and Amnt Backed (Del_P = P_t+1 - P_t, take StDev or Max from list of Del_P's)~~

~~Amount backed on horse as a fraction of total amount backed~~

**Possible Data Sources**

Sectionals & Finish Times: https://www.timeform.com/horse-racing/shop/sectional-times

Tipsters: https://www.tippingsports.com/betting-tips/tips  
https://www.kaggle.com/gunner38/horseracing

Prices: https://historicdata.betfair.com/#/home

Hong Kong: https://www.kaggle.com/gdaley/hkracing  https://www.kaggle.com/hrosebaby/horse-racing-dataset-for-experts-hong-kong
