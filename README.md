# TitanicPredictiveModel
Objective: Use machine learning to create a model that predicts which passengers survived the Titanic shipwreck.

# Solution

Create a correlation matrix. 

# Output

          Pclass       Age     SibSp     Parch      Fare  Survived
Pclass     1.000000 -0.369226  0.083081  0.018443 -0.549500 -0.338481
Age       -0.369226  1.000000 -0.308247 -0.189119  0.096067  0.077221
SibSp      0.083081 -0.308247  1.000000  0.414838  0.159651 -0.035322
Parch      0.018443 -0.189119  0.414838  1.000000  0.216225  0.081629
Fare      -0.549500  0.096067  0.159651  0.216225  1.000000  0.257307
Survived  -0.338481  0.077221 -0.035322  0.081629  0.257307  1.000000

# Findings

Survived vs. Fare: There is a positive correlation (0.2573), indicating that passengers who paid higher fares had a higher chance of survival.

Several factors could explain why passengers who paid higher fares had a higher chance of survival:

Passenger Class (Pclass):
Higher fares are typically associated with higher passenger classes (e.g., 1st class). Passengers in 1st class had better access to lifeboats, were closer to the deck, and were given priority during the evacuation. This likely contributed to their higher survival rate.

Location on the Ship:
Passengers who paid higher fares were often located in better areas of the ship, such as upper decks, which were closer to the lifeboats. This gave them a better chance of reaching safety during the sinking.

Socioeconomic Status:
Passengers who paid higher fares were likely wealthier and may have had better access to resources or influence during the evacuation process.

Family Size:
Passengers who paid higher fares might have traveled with fewer dependents (e.g., smaller families), making it easier for them to evacuate quickly.

# Conclusion

The positive correlation between Survived and Fare suggests that passengers who paid higher fares had a better chance of survival, likely due to factors like passenger class, location on the ship, and socioeconomic status. However, this correlation is only moderate, so fare should be considered alongside other features when analyzing survival patterns in the Titanic dataset.

Correlation Does Not Imply Causation:
Just because higher fares are associated with higher survival rates does not mean that paying a higher fare directly caused survival. Other factors (e.g., passenger class, location on the ship) likely played a role.
Moderate Strength:

The correlation is only 0.2573, which means that fare alone is not a strong predictor of survival. Other features (e.g., Sex, Age, Pclass) are also important.

Outliers:
Some passengers may have paid very high fares but still did not survive, or vice versa. These outliers can affect the correlation.

# Next steps

Meta Modeling - find out which high fare ticket holders had a higher likelihood to survive based on gender or age.

