2023-10-18

## Random Variable

A lot of Machine Learning is concerned with figuring out the probability of an unknown outcome, which in it's simplest form is a random variable.

To backup a bit, it may be helpful to explain what a variable is. A variable is a symbol that represents an unknown mathematical object, which is very wordy for something we've seen  all over the place before. For example: x+1=2 has a variable 'x'.

We have variables just so we can reference to a mathematical object without specifically naming it. This comes in really handy when we want to generalize an equation over all possible situations. For example if you only had $5 and a banana cost $1, you could solve for how many bananas you could by like this: 1*x <= 5 where x = # of bananas. However, you're traveling a lot, so you see a lot of different banana prices and your $5 is worth much more in some of the other countries you're visiting. So if you wanted to take a banana formula with you, you could just exchange the numbers you had for money you have and banana cost for variables. So instead it would be: p*x <= w where p = price of banana, x = # of bananas, and w = amount of money you have. Thanks variables!


Attempting to transition to random variables, the first question that seems to come up is, what makes a variable 'random'? Variables become random when they come as a result of a random process. That appears to just be repeating words so let's try again. If we think about the banana example again, how would we go about figuring out the two variables of interest: the prices of bananas and your corresponding $5 spending power in different countries. We'd visit each of course! Jk, we'd Bing it (that actually does have a nicer ring to it than Google it). 

What we would get then is a dictionary like mapping of the price in different scenarios, but this prices is fixed (we're assuming you're just concerned with the variables values right now). 

picture of mapping here


So if I asked you how many bananas you can buy in the Phillippines you could tell me with certainty.


Ah, there lies the difference. Random variables in contrast we can't tell you with certainty what the values are but instead we talk about them in probabilities. The random variable maps outcomes to a number



How can we really talk about random variables?

The tricky thing is how we think about linear regression's input variables, are these random variables or just plain old variables? 
