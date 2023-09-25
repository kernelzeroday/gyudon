#Gyudon Sake Bourbon Conversion Calculator


To check if using one or two tablespoons of water is more suitable, let’s first convert tablespoons to milliliters. Approximately, 1 tablespoon is equivalent to about 14.79 milliliters (mL). Now, let's see if adding 1 or 2 tablespoons of water to 1 tablespoon of whiskey will yield an ABV in the range of sake (13%-17%).

Let’s assume we have a tablespoon of whiskey, and we know its ABV is 40%. Let's calculate the resulting ABV for both scenarios.

### Scenario 1: 1 Tablespoon of Whiskey + 1 Tablespoon of Water
1. The original volume of whiskey is 14.79 mL.
2. We will add one tablespoon of water, so the final volume will be \( 14.79 \text{ mL} + 14.79 \text{ mL} = 29.58 \text{ mL} \).

\[ \text{ABV}_{\text{final}} = \frac{\text{Volume}_{\text{original}} \times \text{ABV}_{\text{original}}}{\text{Volume}_{\text{final}}} \]
\[ \text{ABV}_{\text{final}} = \frac{14.79 \text{ mL} \times 0.40}{29.58 \text{ mL}} \approx 0.20 \text{ or } 20\% \]

### Scenario 2: 1 Tablespoon of Whiskey + 2 Tablespoons of Water
1. The original volume of whiskey is 14.79 mL.
2. We will add two tablespoons of water, so the final volume will be \( 14.79 \text{ mL} + 2 \times 14.79 \text{ mL} = 44.37 \text{ mL} \).

\[ \text{ABV}_{\text{final}} = \frac{14.79 \text{ mL} \times 0.40}{44.37 \text{ mL}} \approx 0.133 \text{ or } 13.3\% \]

### Result:
Adding 2 tablespoons of water to 1 tablespoon of 40% ABV whiskey will give you a mixture with approximately 13.3% ABV, which is within the ABV range for sake.

### Python Code:
If you want to calculate it in Python, you can use the following code:

```python
# Define the original volume and ABV
volume_original = 14.79  # 1 tablespoon in mL
abv_original = 0.40  # 40%

# Scenario 1: Adding 1 tablespoon of water
volume_final_1 = volume_original + 14.79  # adding 1 tablespoon of water
abv_final_1 = (volume_original * abv_original) / volume_final_1

# Scenario 2: Adding 2 tablespoons of water
volume_final_2 = volume_original + (2 * 14.79)  # adding 2 tablespoons of water
abv_final_2 = (volume_original * abv_original) / volume_final_2

print(f"Scenario 1: Adding 1 tablespoon of water results in {abv_final_1 * 100:.2f}% ABV.")
print(f"Scenario 2: Adding 2 tablespoons of water results in {abv_final_2 * 100:.2f}% ABV.")
```

Executing this code will give you the final ABV for each scenario.





Based on this theoretical model:


When diluting an alcoholic beverage with water, you use the following equation, which is based on the conservation of mass principle:

\[ \text{Volume}_{\text{original}} \times \text{ABV}_{\text{original}} = \text{Volume}_{\text{final}} \times \text{ABV}_{\text{final}} \]

Where:
- \( \text{Volume}_{\text{original}} \) is the original volume of alcohol you have.
- \( \text{ABV}_{\text{original}} \) is the Alcohol by Volume percentage of the original alcohol (expressed as a decimal, so 40% ABV would be 0.40).
- \( \text{Volume}_{\text{final}} \) is the total final volume after dilution.
- \( \text{ABV}_{\text{final}} \) is the desired Alcohol by Volume percentage after dilution (expressed as a decimal).

You can rearrange the equation to find out how much water you need to add to the whiskey to achieve the desired ABV:

\[ \text{Volume}_{\text{final}} = \frac{\text{Volume}_{\text{original}} \times \text{ABV}_{\text{original}}}{\text{ABV}_{\text{final}}} \]

\[ \text{Volume}_{\text{water}} = \text{Volume}_{\text{final}} - \text{Volume}_{\text{original}} \]

### Example:

Let's say you have 100 mL of whiskey (40% ABV), and you want to dilute it to have the ABV of sake, let's use 15% as an average value for sake ABV.

1. Convert the ABV values to decimal form:  
   Whiskey: \( 0.40 \)  
   Sake: \( 0.15 \)

2. Calculate the final volume of the diluted whiskey:
   \[ \text{Volume}_{\text{final}} = \frac{100 \text{ mL} \times 0.40}{0.15} \approx 267 \text{ mL} \]

3. Find out how much water is needed:
   \[ \text{Volume}_{\text{water}} = 267 \text{ mL} - 100 \text{ mL} = 167 \text{ mL} \]

So, you would need to add approximately 167 mL of water to 100 mL of 40% ABV whiskey to dilute it to approximately 15% ABV, resembling sake.

Here's how you might do it in Python:

```python
# Define the original volume and ABV
volume_original = 100  # in mL
abv_original = 0.40  # 40%

# Define the desired final ABV
abv_final = 0.15  # 15%

# Calculate the final volume and the amount of water needed
volume_final = (volume_original * abv_original) / abv_final
volume_water = volume_final - volume_original

print(f"To achieve an ABV of {abv_final * 100}%, you would need to add approximately {volume_water:.2f} mL of water to {volume_original} mL of {abv_original * 100}% ABV whiskey.")
```

This would give you the final volume of the mixture and the amount of water you would need to add to the original whiskey to achieve a 15% ABV.



