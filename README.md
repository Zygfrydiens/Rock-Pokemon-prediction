# Using various machine learning algorithms for ock type pokemon prediction

## In this notebook:
- **About the dataset**
- **Project**
    - Libraries
    - Loading data
    - Molding data
    - Correlation heatmap
    - Checking for missing values
    - Class distribution
    - Splitting data
    - **Naive Bayes**
        - Building the model
        - Model evaluation
    - **Random Forest**
        - Building the model
        - Model evaluation
    - **Logistic Regression**
        - Building the model
        - Model evaluation
    - **Logistic Regression cross-validation (k-fold)**
        - Building the model
        - Model evaluation
    - **Artificial Neuron Network**
        - Normalising data
        - Building the model
        - Model evaluation 
    - Visualisation
    - Conclusions



# About the dataset


Pokemon (also known as Pocket Monsters) is a video game series produced in Japan by GameFreak. First published in 1996 game was huge succes and start of huge franchise. In Pokemon world creatures have different types. Fire, water, grass and many others. Every Pokemon has it's unique stats describing it's species: HP - Health, Attack - physical attack strength, Defense - resistance for physical attacks, Sp.Atk - elemental attack strength, Sp.Def - resistance for elemental attacks and Speed - how quickly it attacks. 

This data set includes 721 Pokemon, including their number, name, first and second type, and basic stats: HP, Attack, Defense, Special Attack, Special Defense, and Speed. It has been of great use when teaching statistics to kids. With certain types you can also give a geeky introduction to machine learning.

This are the raw attributes that are used for calculating how much damage an attack will do in the games. This dataset is about the pokemon games (NOT pokemon cards or Pokemon Go).

The data as described by Myles O'Neill is:

* #: ID for each pokemon
* Name: Name of each pokemon
* Type 1: Each pokemon has a type, this determines weakness/resistance to attacks
* Type 2: Some pokemon are dual type and have 2
* Total: sum of all stats that come after this, a general guide to how strong a pokemon is
* HP: hit points, or health, defines how much damage a pokemon can withstand before fainting
* Attack: the base modifier for normal attacks (eg. Scratch, Punch)
* Defense: the base damage resistance against normal attacks
* SP Atk: special attack, the base modifier for special attacks (e.g. fire blast, bubble beam)
* SP Def: the base damage resistance against special attacks
* Speed: determines which pokemon attacks first each round

The data for this table has been acquired from several different sites, including:

* pokemon.com
* pokemondb
* bulbapedia

This dataset comes from Kaggle (https://www.kaggle.com/abcsds/pokemon)