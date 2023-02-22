# financial-engineering-final-project

Final project of a financial engineering course I had during my exchange semester at Yonsei University, in fall 2022. 

Lookback options are a special type of options, falling into the category of exotic options due to their complexity. Like all option contracts, they provide, at the time of maturity, the right to buy the option’s underlying stock. However, unlike vanilla options, the payoff of the option is path dependent: the payoff is determined using the maximum or minimum price achieved by the underlying stock over the life of the option.

There are two types of lookback options: with floating strike, and with fixed strike. The first type’s strike price is only known at maturity, and is the optimal (max or min) price of the stock over the option’s life. The payoff is then the difference between the floating strike price, and the market price at maturity. The second type of lookback options, the one with fixed strike price, uses as the name implies a predetermined strike price, and its payoff is the difference between this fixed strike price and the asset’s optimal price observed during the option’s life.

In this project, we will try to perform hedging of both types of lookback options. Since there is no closed formula for the pricing of fixed strike lookback options, we cannot perform delta hedging using the Black-Scholes model, like we could do with vanilla options. Therefore, this project will aim at performing hedging using Deep Learning to compute the delta at each time step.
