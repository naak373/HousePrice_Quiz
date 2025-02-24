Interpretation 
The Best Performing Model is the Random Forest Model
Random Forest measures the importance of its features by how much they actually tend to reduce error (impurity) in its associated decision trees.
More specifically, important variables will have a higher rank in the tree, 
usually appearing very frequently at a higher level where they cause significant contributions toward the prediction improvements.

OverallQual (35%): It is the most important factor-the quality of materials and finishes of a house, 
and it is quite intuitive in real life-more well-built houses invariably-more expensive houses. 
GrLivArea (18%): Again, the whole living area matters quite a lot. Most living areas increase the value of homes. 
GarageCars (12%): Concerning how many cars the garage holds, this is important because larger garages increase property desirability. 
TotalBsmtSF (10%): A finished basement indeed adds much value, as buyers would expect. 
YearBuilt (8%): Newly built houses tend to have more modern features and require less repairing, making them high on the market value.

These rankings of features according to importance are in concert with the way properties are valued in reality:

Real-World Alignment
Priority is given to quality, space, and modernity by buyers.
Some features, such as garage size, basement size, and year built, reflect the practicality of home buying.
Perhaps not much in the influencing game are features of lesser importance (pool presence, kitchen quality, etc.);
yet, they still do matter but to a much smaller extent when it comes to the variations in price.

Bonus Challenge 
1. Generative Models are not for Simple Numbers but by a Distribution of Data They Create
A GAN or VAE learns to learn from the inherent data distribution and generate new syntactic samples, e.g., samples that resemble training data.
But, in reality, we expect exact numbers as outputs, house price, for example, rather than data that looks realistic.
For instance, a GAN could produce realistic features of a house but would be unable to generate a numeric output for a price prediction of a given house.

3. No Direct Supervised Learning to Learn Number Targets. 
Regression modelling essentially means supervised learning, where there is a one to one mapping between some input features, square footage and no of rooms, to a unique output that will be some numeric attribute, e.g., house price. 
GANs and VAEs do not natively optimize for losses intended for regression, such as Mean Squared Error or Mean Absolute Error. Rather, the generative loss, which is not meant to make predictions look as accurate as possible, is minimized.
