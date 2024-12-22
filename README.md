# AGE-DURATION-CALCULATOR
Project Overview

The objective of this project is to calculate the total duration a person has lived based on their age in years. The application allows users to choose a time unit (e.g., months, weeks, days, hours, minutes, or seconds) to see the result in the desired format. The program is designed to be interactive, user-friendly, and error-free.
Thought Process During Development

1. Understanding the Problem

The first step was to understand the requirements:

Input: The age of a person in years.

Output: The age converted into a specific time unit chosen by the user.

Constraints: The program should support six time units, be user-friendly, and handle invalid inputs gracefully.

2. Structuring the Code

To ensure clarity, reusability, and separation of concerns, I decided to:

Use a class (AgeDurationCalculator) to encapsulate the logic for calculating durations. This makes the code modular and easy to expand in the future.

Write the interactive logic in a separate main() function for better separation between computation and user interaction.

3. Conversion Factors

To compute the duration in different units, I listed the conversion factors:

1 year = 12 months
1 year ≈ 52.1775 weeks (considering leap years)
1 year = 365.25 days (average year length accounting for leap years)
1 day = 24 hours, 1 hour = 60 minutes, and 1 minute = 60 seconds.
These factors were stored directly in the calculate_duration method for simplicity.

4. User Input Handling

User input was designed to be intuitive:
For age, a positive integer is required.
For time unit selection, users can input either the full name (e.g., "months") or the first letter/abbreviation (e.g., "m" for months, "min" for minutes).
I used a mapping (unit_map) to translate shorthand inputs into their full forms.

5. Error Handling
Anticipating potential errors (e.g., negative age or invalid time unit), I included:
A check to ensure the age is a non-negative integer.
A fallback message if the user enters an invalid time unit.

6. Output Formatting

The result is displayed in a clean format:

Time unit names are capitalized for readability.
The result is rounded to two decimal places for accuracy and simplicity.

How to Use

1. Run the program.
2. Enter your age in years when prompted.
3. Select a time unit by typing either its full name or shorthand.
4. View the result, which displays how long you have lived in the chosen unit.

Thought Process Summary

My goal was to ensure that the program is easy to use, accurate in calculations, and robust against invalid inputs. By structuring the code modularly and handling edge cases carefully, I aimed to create a solution that balances functionality and simplicity.
