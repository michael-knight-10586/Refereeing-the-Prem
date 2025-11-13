# Refereeing-the-Prem: Reflexivity in refereeing performance

This project asks how Premier League refereeing performance is influenced by recent events. It is designed to include a range of Azure Databricks features that support production level code.

## Hypothesis

Do referees officiate each game independently of their own recent performances or do they compensate in some way? In an ideal world referees would make decisions correctly and independently of outside factors, such as recent events or their own recent performance. But in the real world we can rank referees by performance over any number of games. For any Premier league match we have bookmakers' odds on the likely number of red and yellow cards from which we derive an implied probability of the sum of each. In any given game the referee will brandish more or less than an expected average. This will largely be due to the randomness of in-game events. Over time we can create a league table of referee performance where we rank officials from highest to lowest in the propensity to punish players compared to expectation.

In reviewing games the Premier League Game Match officials analyse decision-making for errors and feeback to referees. Their performance/ability should be measured by their handling of events rather than how they conform to an expected average. But how are referees really thought of? Who gets the lucrative Champions League or World Cup roles? And how does a referee react to officiating a 'bloodbath' one week or brandishing fewer cards than his colleagues over a number of matches? My guess is that there is some reflexivity or unconscious desire to regress-to-the-mean in the number of punishments they dish out. Referees who have dealt more cards than expected are likely thought of as over-zealous and at the other extreme too cautious. My guess is that to succeed it behoves the ambitious referee to sit in the middle. In any recent run of games where a referee veers from expected average we should find a small but detectable response in the opposite direction.

## Usage

This is part of a wider project that takes freely available football match data and creates benchmark models through machine learning. We could use this as the basis of a betting strategy. More likely the effect we will be too small among other factors to create an edge over the market and the bookmakers' over-round. 
Here I want to publish a simple model on a subset where we can see the full process in Azure Databricks for CI/CD where our output is probabilities for sports traders.

## Technologies Used
* Azure Data Lake Storage
* Azure Databricks
* Power BI

## Machine Learning

The aim here is a simplicity of design and for results. We are interested in only one factor; the effect of recent performance and I will use logistic regression.
