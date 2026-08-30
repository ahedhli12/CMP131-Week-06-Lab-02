# CMP 131 – Python Programming


> **Required file location:** Keep every Python file directly in the repository root. Do not create a `src` folder.

## Week 6 – Lab 2: Temperature Clothing Recommendation

**Total Points: 100**

**Optional Bonus: Up to 10 Points**

## Learning Objectives

After completing this lab, students should be able to:

* Accept numeric and text input from the user.
* Convert user input to an appropriate data type.
* Use `if`, `elif`, and `else` statements.
* Compare a value against multiple ranges.
* Correctly handle temperature boundary values.
* Use string methods to standardize text input.
* Display clear recommendations based on user input.
* Test a program using different input values.
* Use comments to explain the major sections of a program.

## Assignment Overview

Create a Python program that asks the user to enter the current temperature in degrees Celsius.

The program will use conditional statements to provide a clothing recommendation based on the temperature entered.

Use the following recommendations:

| Temperature       | Recommendation      |
| ----------------- | ------------------- |
| Below 0°C         | Wear a heavy coat   |
| 0°C to below 15°C | Wear a jacket       |
| 15°C through 25°C | Wear a sweater      |
| Above 25°C        | Wear light clothing |

The program must display the temperature entered by the user and the appropriate clothing recommendation.

For the optional bonus challenge, ask the user to enter their favorite season and display a personalized message based on the response.

The instructor is not providing completed Python code or an exact output design. Students must design, write, and test their own programs.

## Required Python File

Create a Python file named:

`temperature_recommendation.py`

Include a comment header at the beginning of the file containing:

* Student name
* Course number
* Week number
* Lab number
* Assignment title
* Date

## Part 1: Display a Program Title

Display a descriptive title when the program begins.

The title should clearly indicate that the program provides clothing recommendations based on the current temperature.

Use appropriate spacing or decorative characters to make the title easy to identify.

Possible decorative characters include:

* Equal signs
* Hyphens
* Asterisks
* Number signs

Students should create their own title and output design.

## Part 2: Temperature Input

Ask the user to enter the current temperature in degrees Celsius.

The temperature may be:

* A positive value
* A negative value
* Zero
* A decimal value

Convert the user’s input to an appropriate numeric data type before using it in a comparison.

Store the temperature in a meaningfully named variable.

Examples of valid temperature values include:

* `-10`
* `0`
* `8.5`
* `15`
* `22.5`
* `25`
* `31`

## Part 3: Determine the Clothing Recommendation

Use an `if`, `elif`, and `else` structure to determine the appropriate clothing recommendation.

The program must select and display only one recommendation.

### Below 0°C

If the temperature is below `0°C`, recommend wearing a heavy coat.

### From 0°C to Below 15°C

If the temperature is at least `0°C` but below `15°C`, recommend wearing a jacket.

### From 15°C Through 25°C

If the temperature is at least `15°C` and no more than `25°C`, recommend wearing a sweater.

### Above 25°C

If the temperature is above `25°C`, recommend wearing light clothing.

## Important Boundary Values

The program must correctly handle the boundary values.

* `-0.1°C` → Heavy coat
* `0°C` → Jacket
* `14.9°C` → Jacket
* `15°C` → Sweater
* `25°C` → Sweater
* `25.1°C` → Light clothing

Every temperature must produce exactly one clothing recommendation.

## Part 4: Display the Result

Display:

* The temperature entered by the user
* The Celsius symbol or abbreviation
* The appropriate clothing recommendation

The result should be written as a complete and clear message.

The output must:

* Use clear labels.
* Include appropriate spacing.
* Use consistent capitalization.
* Display only one clothing recommendation.
* Be easy for the user to understand.

Students should create their own output wording and design.

## Optional Bonus Challenge: Favorite Season

**Up to 10 Bonus Points**

After displaying the clothing recommendation, ask the user to enter their favorite season.

The program should recognize the following seasons:

* Spring
* Summer
* Fall
* Winter

Use conditional statements to display a different personalized message for each season.

For example, the message may mention:

* Flowers or warmer weather for spring
* Sunshine or outdoor activities for summer
* Colorful leaves or cooler weather for fall
* Snow or cold-weather activities for winter

Students must create their own personalized messages.

### Bonus Input Requirements

The season input should work whether the user enters uppercase or lowercase letters.

For example, the following entries should be treated as the same season:

* `summer`
* `Summer`
* `SUMMER`

Use a Python string method to standardize the user’s response before comparing it.

If the user enters something other than the four listed seasons, display a friendly message explaining that the season was not recognized.

## Code Comments

Use comments to identify and explain the major sections of the program.

Include comments for:

* The program information header
* The program title
* The temperature input section
* The temperature conditional statements
* The clothing recommendation output
* The optional favorite-season input
* The optional season conditional statements
* The optional personalized message

Comments should briefly explain the purpose of each major section. They do not need to repeat every Python statement word for word.

## Required Testing

Test the program using all the following temperature values.

### Test 1: Below Freezing

Enter:

`-10`

Expected recommendation:

`Wear a heavy coat`

### Test 2: Heavy-Coat Boundary Check

Enter:

`-0.1`

Expected recommendation:

`Wear a heavy coat`

### Test 3: Jacket Lower Boundary

Enter:

`0`

Expected recommendation:

`Wear a jacket`

### Test 4: Jacket Range

Enter:

`8`

Expected recommendation:

`Wear a jacket`

### Test 5: Jacket Upper Boundary Check

Enter:

`14.9`

Expected recommendation:

`Wear a jacket`

### Test 6: Sweater Lower Boundary

Enter:

`15`

Expected recommendation:

`Wear a sweater`

### Test 7: Sweater Range

Enter:

`20`

Expected recommendation:

`Wear a sweater`

### Test 8: Sweater Upper Boundary

Enter:

`25`

Expected recommendation:

`Wear a sweater`

### Test 9: Light-Clothing Boundary Check

Enter:

`25.1`

Expected recommendation:

`Wear light clothing`

### Test 10: Warm Temperature

Enter:

`32`

Expected recommendation:

`Wear light clothing`

Confirm that:

* Every test produces the correct recommendation.
* Only one recommendation is displayed for each temperature.
* Boundary values are handled correctly.
* The program runs without errors.

## Bonus Testing

If completing the bonus challenge, test all the following entries:

* `Spring`
* `summer`
* `FALL`
* `Winter`
* `rainy`

Confirm that:

* Each valid season produces a different personalized message.
* Capitalization does not affect the result.
* An unrecognized-season message is displayed for `rainy`.
* The program runs without errors.

## Point Distribution

* Program title and clear temperature prompt: 10 points
* Correct numeric input conversion: 10 points
* Correct heavy-coat condition: 15 points
* Correct jacket condition: 15 points
* Correct sweater condition: 15 points
* Correct light-clothing condition: 15 points
* Clear and properly formatted output: 10 points
* Comment header and code comments: 5 points
* Successful testing and correct boundary handling: 5 points

**Required Assignment Total: 100 points**

### Bonus Point Distribution

* Ask the user for a favorite season: 2 points
* Standardize capitalization correctly: 2 points
* Correctly recognize all four seasons: 2 points
* Display a different personalized message for each season: 2 points
* Handle an unrecognized season: 2 points

**Maximum Bonus: 10 points**

## Functional Requirements

When the program runs, it must:

* Display a descriptive program title.
* Ask the user to enter a temperature in Celsius.
* Accept whole-number and decimal temperatures.
* Accept positive and negative temperatures.
* Convert the temperature to an appropriate numeric data type.
* Use `if`, `elif`, and `else` statements.
* Recommend a heavy coat for temperatures below `0°C`.
* Recommend a jacket for temperatures from `0°C` to below `15°C`.
* Recommend a sweater for temperatures from `15°C` through `25°C`.
* Recommend light clothing for temperatures above `25°C`.
* Display the entered temperature.
* Display only one clothing recommendation.
* Correctly handle all boundary values.
* Include comments explaining the major sections.
* Run completely without errors.

If completing the bonus challenge, the program must also:

* Ask the user for their favorite season.
* Recognize spring, summer, fall, and winter.
* Accept different capitalization styles.
* Display a personalized message for each season.
* Display a friendly message when the season is not recognized.

## General Requirements

* Use Python to complete the assignment.
* Save the program as `temperature_recommendation.py`.
* Use meaningful and consistent variable names.
* Use a clear input prompt.
* Convert the temperature to an appropriate numeric data type.
* Use an `if`, `elif`, and `else` structure.
* Use the required temperature ranges.
* Display only one clothing recommendation.
* Include the required comment header.
* Include comments explaining the major sections.
* Use clear headings, labels, and messages.
* Test all required temperature values.
* Check spelling, capitalization, grammar, and punctuation.
* Make sure the program runs without errors.
* Follow the course AI-use policy.
* Record any AI assistance in `AI-Use-Report.md`.

## Required Organization

Organize the assignment as follows:

* `Week-06`

  * `Lab-02`

    * `CMP131-Week-06-Lab-0.md2.md`
    * `AI-Use-Report.md`
    * `src`

      * `temperature_recommendation.py`

## Submission Requirements

Submit or push the complete `Lab-02` folder.

The submission must include:

* `temperature_recommendation.py`
* `AI-Use-Report.md`

Before submitting, verify that:

* The required Python file is included.
* The filename is exactly `temperature_recommendation.py`.
* The program contains a complete comment header.
* The program contains comments explaining each major section.
* The program asks for a Celsius temperature.
* The temperature input is converted to an appropriate numeric data type.
* The program uses `if`, `elif`, and `else`.
* All four temperature ranges work correctly.
* All boundary values are handled correctly.
* The program displays only one clothing recommendation.
* The output is clear and appropriately formatted.
* The program was tested using all required values.
* The program runs without errors.
* The AI-use report is complete.
* The latest work has been committed and pushed to GitHub.

If completing the bonus challenge, also verify that:

* The program asks for the user’s favorite season.
* All four seasons are recognized.
* Different capitalization styles are accepted.
* Each season produces an appropriate personalized message.
* An invalid or unrecognized season is handled appropriately.

## Suggested Git Commit Messages

* Create Week 6 Lab 2 Python file
* Add Celsius temperature input
* Add clothing recommendation conditions
* Test temperature boundary values
* Add favorite season bonus
* Add season personalization messages
* Improve output formatting and comments
* Complete Week 6 Python lab

---

## GitHub Starter Repository

Use the following public starter repository:

[CMP131-Week-06-Lab-02](https://github.com/ahedhli12/CMP131-Week-06-Lab-02)

### Getting Started

1. Open the starter repository using the link above.
2. If **Use this template** is available, select **Use this template → Create a new repository**.
3. Choose your personal GitHub account as the owner.
4. Name your repository `LastName-FirstName-CMP131-Week-06-Lab-02`.
5. Set your repository to **Public**.
6. Clone your own newly created repository—not the instructor’s starter repository.
7. Open the entire cloned folder in Visual Studio Code.
8. Complete and test every required Python file.
9. Commit and push your work to GitHub.
10. Verify that your latest files appear on GitHub.
11. Complete `AI-Use-Report.md`.
12. Submit the required work through Blackboard Ultra and include your public repository link when requested.

### Required Repository Files

- `CMP131-Week-06-Lab-02.md`
- `AI-Use-Policy.md`
- `AI-Use-Report.md`
- `temperature_recommendation.py`

### Before You Submit

- [ ] All required Python files are in the repository root.
- [ ] Every required filename is exact.
- [ ] Each program runs successfully.
- [ ] Required tests and screenshots are complete.
- [ ] `AI-Use-Report.md` is complete and accurate.
- [ ] The latest commit is visible on GitHub.
