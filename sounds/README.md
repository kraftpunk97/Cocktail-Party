# Cocktail Party Problem using Fourth Order Blind Identification(FOBI)

## Premise
You are at a party, trying to rizz up this gorgeous woman. You tell a few jokes, and you can tell that she's into you. You want to keep the conversation going but all the noise is making it difficult for you to understand what the mother of your future children is saying to you. How do you focus on her voice and tune out the noise?

This is the "Cocktail Party Problem", a source separation problem from signal processing. Here, we demonstrate the use of the "Fourth Order Blind Identification" algorithm to separate out the sources from a data received by different sensors (the microphones). 


## Why Fourth order?
So I'm not really familiar with DSP, I just like the challenge posed by the Cocktail Party Problem (which is why you're reading this document), but from what I understand, for most of the things, Gaussian distribution, or an approximation of the Gaussian gives a satisfactory result. So for the most part, poeple are content with first-order (mean) and second-order (variance) information. That being said, sound waves are not really Gaussian. So because sound waves are much more complex than what a Gaussian model could describe, we need to go beyond second-order information statistics. Apparently even the third order statistics weren't enough (otherwise they wouldn't have gone to fourth). Hence, we find ourselves dealing with fourth order statistics. 


## Sources

The Fourth Order Blind Identification algorithm is described in this [paper](https://perso.univ-rennes1.fr/laurent.albera/alberasiteweb/pdf/FerrAC03-ICASSP.pdf).