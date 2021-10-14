This simulator is intended to be a tool to help students (within academia or not; we're all students of life and seeking knowledge, right?) strengthen their intuition with regards to randomization in the context of randomized controlled trials (aka, field experiments).

#### The Basic World of this Simulator

This simulator constructs a simplified world with the following characteristics:

* A finite set of experimental subjects (you control how many)
* A "treatment" for which we want to detect the impact (you get to be omnipotent and specify the effect of the treatment)
* A single covariate--represented by "color" (you control the number of levels)

#### Treatment

The treatment is (intentionally) not specified. It could be anything that you could, in theory, apply to the subjects through _random assignment_: exposure to social media advertising, sending a promotional email, knocking on a door as part of political canvassing, etc. Use your imagination!

**An important note on "subjects":** these do _not_ have to be thought of as "individual human beings." They can be groups of people. For instance, for advertising as a treatment, they could be DMAs or zip codes. 

#### Effect

Impact, similarly, is (intentionally) not specified. There is a "base" (untreated) value of 1,000, but that's then transformed and had noise introduced into it based on the different simulator settings. As such, the (omnipotent) effect is a value set as a percentage, and the results of the simulations of "observed effects" are also represented as percentages--as the "% increase" as the effect of the treatment.

The minimal effect that can be specified is 0% just...because. It would likely handle a negative impact just fine, but that's not pedagogically productive to introduce as an option.

#### "Color" Represents a Covariate

The simulator uses "color" to represent a heterogeneous covariate within the population. This is _not_ the treatment. It's just some other characteristic of the subjects. RCTs inherently have to deal with all manner of "unobserved heterogeneity," which is just to say that there will be oodles of characteristics of the subjects that differ across the population: household income, race, age group, past experiences with a product, geographic region, etc.

_This is where randomization is so stinkin' cool_. We don't _have_ to account for all of these variables. If we truly work with "random assignment," then, given sufficient data, all of these differences effectively cancel each other out across our treated and untreated groups.

Having said that, this simulator is intended to enable the exploration of different aspects of covariates. We're working with only a single covariate here (color), but we can explore it through many different lenses:

* Is it a covariate that we can actually know about and factor in to our experimental design (i.e., conduct random assignment _within "blocks"_ where the subjects are grouped together based on having similar/same values for the covariate)
* Is the covariate predictive of the outcome (effect)? For instance, household income could be a covariate that can be used to predict how much will be spent on a new car. But, the treatment of interest is actually "exposure to advertising." Conversely, another covariate could be hair color, which has not expected predictive value when it comes to how much will be spent on a new car. _Both_ of these would be potential heterogeneous covariates.