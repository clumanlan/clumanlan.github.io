2023-10-18

## Random Variables

A lot of stasitical modeling is concerned with figuring out the probability ditribution of an outcome, which is really just a random variable.

To backup a bit, it may be helpful to explain what a variable is. A variable is a symbol that represents an unknown mathematical object. The reason we use variables is so that we can reference a mathematical object without specifically giving it a number.

For example: x+1=2 has a variable 'x'. 

Using a variable in this situation seems rather pointless since there is really only one value the variable can be, 3 (lol jk). However, variables become really handy when we want to generalize an equation over all possible situations. For example, let's say you only had $5 and a banana cost $1, you could solve for how many bananas you could by like this: 1*x <= 5 where x = # of bananas. However, you're potentially traveling to different countries so you could see a lot of different banana prices. So if you wanted to take a banana formula with you, you could just exchange the numbers price and number banans with variables. So instead it would be: p*x <= 5 where p = price of banana and x = # of bananas Thanks variables!


Attempting to transition to random variables, the first question that seems to come up is, what makes a variable 'random'? Variables become random when they come as a result of a random process. That appears to just be repeating words so let's try again. If we think about the banana example again, how would we go about figuring out variable of interest (the price of bananas in each country). We'd visit each of course! Jk, we'd Bing it (that actually does have a nicer ring to it than Google it). 


Let's say we only have four countries we're going to potentially travel to: Phillippines, Japan, Netherlands or another city in the US. So we can draw up the potential outcomes of our journey.

![sample space of countries](/docs/assets/2023-10-18/0-country-sample-space.png)



We can then take what we learned from our bing search and map (or assign) each country to their corresponding banana price. 

![sample space of countries with mapping](/docs/assets/2023-10-18/1-country-sample-space-mapping.png)


I'm making this up. That being said the function of mapping (i.e. 'P') that we did here is what defines what a random variable is.


The really confusing part is that 'random' doesn't mean random in the strict sense, where it's truly unpredictable and without pattern (also a lot of debate whether there is anything that is actually random). Instead, 'random' references to the fact that it comes from uncertain outcomes and the function of mapping from these outcomes to a number  (i.e. 'P'), is what a random variable is. The uncertainity lies in the outcome of the experiment (i.e. it's not clear which country you're going to visit).


It becomes more clear if we add additional uncertainty, like let's say we're uncertain of when we're going on our banana exploration trip. We're either going this year or next and we can only go to Netherlands next year due to budget.

We would expand the white box then to have multiple observations or outcomes related to each country, with each outcome representing both a country and year that we visit.

![sample space of countries with year](/docs/assets/2023-10-18/2-country-sample-space-w-year.png)

To be clear the white box that the circles sit inside is called a sample space. A sample space simply contains possible outcomes of an experiment. Each possible outcome in a sample space is mutually exclusive (e.g. you can't visit two countries at the same time) and collectively exhuastive (e.g. we have a complete list of possible countries we can visit and when).

We can then map these to another random variable that's a function of year.

![sample space of countries with year mapping](/docs/assets/2023-10-18/3-country-sample-space-w-year-mapping.png)


We could define it like this: 

These is a discrete random variable with finite set out of outcomes called a BLAH BLAH BLAH




We could've changed it so rather than years it was this year or not this year thereby becoming a Poisson Distribution (distribution with 0, 1)

PICTURE OF BINS

probability mass function description here.



In this example we have multiple values mapped to 2023





each random variable has a probability distribution and from what we know from the distribution model the space







Continous random variable. 

Random variables are neat because really just referencing to things that we're trying to figure out. It's a bit interesting to think about sample space as well, just like all possible outcomes.


DISCRETE RANDOM VARIABLE PROBABILITY MASS FUNCTION

PROBABILITY DENSITY FUNCTION
Last pieces: 
- you add visuals
- understand what a probability distribution of a discrete random variable is
- 

The tricky thing is how we think about linear regression's input variables, are these random variables or just plain old variables? I guess for next time, or never, we'll see.

