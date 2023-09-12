2023-08-25

## Bayes Theorem


Probability is always easier with examples, especially engaging ones.

For this we'll picture you're a short Asian guy on a dating app (aka me off and on several years ago). 
After reading this depressing [article](https://theconversation.com/asian-guys-stereotyped-and-excluded-in-online-dating-130855) you come to realize that 90% of non-Asian women want nothing to do with you (romantically that is). Yet you continue swiping with a false feeling that you're special, with your current odds of being 10% chance of matching if the person is non-Asian (successful assimilation has made you primarily attracted to non-Asian females).

For sake of argument and because a 10% square is tough to visualize we'll say that the new influx of Asian movies and superheros has doubled the chance of a non-Asian woman being open to dating an Asian man to 20%, yipee!

As you're swiping you come across an attractive white brunette and after some Instagram sleuthing, you've seen that her ex-boyfriend was Asian (and presumably still is). Hooray! But then you remember you're short.

However, since she's the same height you still have a shot? 51% of women would date men the same height or shorter than them after all based on this [Five Thirty Eight](https://fivethirtyeight.com/features/how-common-is-it-for-a-man-to-be-shorter-than-his-partner/) article you read.


Based on another article (that you can no longer find) you know that 35% of those that are willing to date short guys are also open to date Asians as well.

So given these stats you oddly have memorized and the the new information gained from your Instagram sleuthing (creeping) how have your odds changed?

Let's do some math! 

Or first let's at least diagram what we know.




We start with the whole universe of non-Asian females on a dating app (pretend there's a million dots in the circle that represent women that will very unlikely swipe right).


![universe of females dating on hinge](/docs/assets/2023-09-05/0-universe.png)



We can create two squares in here that represent the small world (or sample) in the universe that date short guys and date Asian guys.

![separated asian and short worlds](/docs/assets/2023-09-05/1-separated_asian_short.png)


Oh, but we forgot of course there's overlap since there are some (not a lot) of non-Asian women out there who will date a guy who is both Asian and short. Let's update our diagram to account for this. 

![joined asian and short worlds](/docs/assets/2023-09-05/2-asian_short_overlap.png)

Neat!


So we've just been defining the sample space through drawing shapes with random sizes, let's apply the evidence we've learned along with some of the weird stats you were stating earlier.


Given, only 51% of women would date a shorter man (this may be inflated but we'll run with it), we can adjust the orange square to cover about half of the cirlce (pretend it's half I'm still working on design ability). 

Also, since we know that 20% of non-Asian women would date an Asian man we'll adjust that square as well to cover about 1/5 of the circle.

![asian and short adjusted size](/docs/assets/2023-09-05/3-asian_shor4_universe_adjusted_size.png)



So we've as a result defined our sample space! Or in other words created squares with areas based on their respective probabilities. Currently we're looking at the whole universe of non-Asian women, but we do know more. 

The new evidence we learned earlier is that your prospective beau is open to dating Asian men due to her past relationship. As a result we can filter down to the world in which women are open to dating Asian men. 

Circled.

![asian and short adjusted size highlighted](/docs/assets/2023-09-05/4-asian_shor4_universe_adjusted_highlighted.png)

Filtered.

![filtered universe](/docs/assets/2023-09-05/5-filtered-universe.png)


So we've updated the world to account for our evidence (that she is open to dating an Asian guy). 


Our updated question becomes, what's the probability that given she dates an Asian guy she dates a short Asian guy (aka you)?

It seems rather simple if we remember that the areas = probabilities. We'd really just want to take the area that represents Asian and short men and divide that by the area of all non-Asian women that date Asian men (since this is the complete filtered world we're currently in). 

So it would look something like this:

![bayes formula setup](/docs/assets/2023-09-05/6-bayes-formula-setup.png)


We need a way to define the filtered area. We simply apply the probabilities that helped us to filter down to this specific scenario in the first place.

![bayes formula setup w probability](/docs/assets/2023-09-05/7-bayes-formula-probability.png)

So you're at a whopping: 90%!


Through the drawing, filtering and applying random stats we just applied the Bayes Theorem. 

**Bayes Theorem**
```math 
    P(A | B) = {P(B|A)  P(A)} \over {P(B)}
```

Where:
-  $`P(A|B)`$ is the posterior probability of event A given event B.
-  $`P(B|A)`$ is the probability of event B given event A.
-  $`P(A)`$ is the prior probability of event A.
-  $`P(B)`$ is the prior probability of event B.


And in our example: 

Where:
-  $`P(Date Short | Date Asian)`$ is the probability of dating a short guy given she's open to dating an Asian guy - what we're trying to figure out
-  $`P(Date Asian | Date Short)`$ is the probability of dating an Asian guy given she dates a short guy - 35%
-  $`P(Date Short)`$ is the prior probability of event A - 51%
-  $`P(Date Asian)`$ is the prior probability of event B - 20%



But you're also broke and live in a basement which there are no squares for in the original circle.






Probbility Ch. 5 Ace Data Science Interview


