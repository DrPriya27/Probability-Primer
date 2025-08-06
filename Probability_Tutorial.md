# Fundamentals of Probability

## Table of Contents
1. [Introduction to Probability](#1-introduction-to-probability)
2. [Types of Probability](#2-types-of-probability)
3. [Real-Life Relevance of Probability](#3-real-life-relevance-of-probability)
4. [Key Properties of Probability (Fundamental Laws)](#4-key-properties-of-probability-fundamental-laws)
5. [More Real-World Examples & Applications](#5-more-real-world-examples--applications)
6. [Permutations](#6-permutations)
7. [Combinations](#7-combinations)
8. [Detailed Explanation: Events in Probability](#8-detailed-explanation-events-in-probability)
9. [Examination Practice Problems](#9-examination-practice-problems)
---

## 1. Introduction to Probability


### What is Probability?
Probability is a measure of the likelihood that a specific event will occur. It quantifies uncertainty by assigning a value between 0 (impossible) and 1 (certain) to events, or equivalently from 0% to 100%. For example, the probability of flipping heads on a fair coin is 0.5 (or 50%). Probability theory provides a systematic way to analyze random phenomena, predict outcomes, and make decisions when outcomes are not guaranteed.

**Real-World Example:**  
Imagine you check the weather forecast and see a 70% chance of rain tomorrow. This means, based on historical data and current conditions, meteorologists estimate that out of 100 similar days, it would rain on about 70 of them. You can use this probability to decide whether to carry an umbrella or plan outdoor activities.

**More Examples:**  
- **Lottery Tickets:** If a lottery has 1,000,000 tickets and only one winning ticket, the probability of winning with a single ticket is 1/1,000,000 (0.000001 or 0.0001%). This helps you understand the odds before buying a ticket.
- **Medical Testing:** If a test for a disease is 99% accurate and the disease occurs in 1% of the population, probability helps doctors interpret test results and make informed diagnoses.
- **Sports:** If a basketball player makes 80% of free throws, the probability of making the next shot is 0.8. Coaches use these probabilities to strategize during games.
- **Quality Control:** In manufacturing, if 2 out of every 100 products are defective, the probability of picking a defective product at random is 2%. This information guides quality improvement efforts.
- **Online Shopping:** If a website says there’s a 95% chance your package will arrive within 3 days, you can use this probability to plan when to expect your delivery.


### Probability as a Fraction, Decimal, and Percentage

Probability can be expressed in three equivalent forms:
- **Fraction:** Shows the ratio of favorable outcomes to total outcomes.
- **Decimal:** Converts the fraction to a decimal value between 0 and 1.
- **Percentage:** Multiplies the decimal by 100 to show probability as a percent.

**Classical Probability Formula:**  
\( P(E) = \frac{\text{Number of favorable outcomes}}{\text{Total number of outcomes}} \)  
Must satisfy: \( 0 \leq P(E) \leq 1 \)

**Example:**  
Suppose you roll a fair six-sided die. What is the probability of rolling a 4?

- **Favorable outcomes:** 1 (only the number 4)
- **Total outcomes:** 6 (numbers 1 through 6)

- **Fraction:**  
    \( P(4) = \frac{1}{6} \)

- **Decimal:**  
    \( P(4) = 1 \div 6 \approx 0.1667 \)

- **Percentage:**  
    \( P(4) = 0.1667 \times 100 \approx 16.67\% \)

So, the probability of rolling a 4 is \( \frac{1}{6} \), or about 0.167, or 16.7%.


**Examples:**

- **Coin Toss:**  
    Probability of getting heads when tossing a fair coin:  
    Favorable outcomes = 1 (heads)  
    Total outcomes = 2 (heads, tails)  
    \( P(\text{Heads}) = \frac{1}{2} = 0.5 \)

- **Rolling a Die:**  
    Probability of rolling an even number on a six-sided die:  
    Favorable outcomes = 3 (2, 4, 6)  
    Total outcomes = 6  
    \( P(\text{Even}) = \frac{3}{6} = 0.5 \)

- **Drawing a Card:**  
    Probability of drawing an Ace from a standard deck of 52 cards:  
    Favorable outcomes = 4 (Aces)  
    Total outcomes = 52  
    \( P(\text{Ace}) = \frac{4}{52} \approx 0.077 \)



### Why Study Probability?
Studying probability is essential for several reasons:
- **Quantifying Uncertainty:** It allows us to measure and manage uncertainty in everyday life and scientific research. Key point: Probability doesn’t tell us exactly what will happen, but it gives us a way to measure and compare how likely different outcomes are. This helps us manage risk and make informed choices.
    *Example:* When tossing a coin, probability quantifies the uncertainty of getting heads or tails (each has a probability of 0.5).

- **Foundation for Statistical Inference:** Probability underpins statistical methods used to draw conclusions from data, estimate parameters, and test hypotheses.  
    *Example:* In clinical trials, probability helps determine if a new drug is effective by analyzing the likelihood that observed results are due to chance.

- **Decision Making:** Probability helps in making informed decisions under risk, such as evaluating insurance policies or investment strategies.  
    *Example:* An investor uses probability to assess the risk of stock price changes before buying shares.

- **Applications Across Industries:** Probability is critical in fields like finance (risk assessment, portfolio management), insurance (premium calculation, claim prediction), medicine (clinical trials, diagnostic testing), engineering (quality control, reliability analysis), and artificial intelligence (machine learning algorithms, predictive modeling).  
    *Example:* Insurance companies use probability to calculate the chance of car accidents and set premiums accordingly.

- **Modeling Random Processes:** It provides tools to model and analyze random events, such as weather forecasting, genetics, and network reliability.  
    *Example:* Meteorologists use probability models to predict the chance of rain based on atmospheric data.

Understanding probability equips you to interpret data, assess risks, and solve problems in a wide range of real-world contexts.

## Basic Terminology
- **Trial:** A single attempt or repetition of an experiment.  
    *Example:* Each time you flip a coin, that flip is one trial.

- **Experiment:** A process or action that can produce different outcomes.  
    *Example:* Flipping a coin 10 times is an experiment; each flip is a trial, and the experiment consists of all 10 flips.

- **Outcome:** A single possible result of an experiment.  
    *Example:* Getting a 4 when rolling a die is an outcome.

- **Sample Space (S):** The set of all possible outcomes.  
    *Example:* For rolling a die, S = {1, 2, 3, 4, 5, 6}.

- **Event (E):** One or more outcomes from the sample space.  
    *Example:* Getting an even number when rolling a die is an event, E = {2, 4, 6}.

**Demonstrative Examples:**

- If you flip a coin three times:
    - Each flip is a trial.
    - The experiment is "flip a coin three times."
    - Possible outcomes for one flip: Heads or Tails.
    - Sample space for three flips: {HHH, HHT, HTH, HTT, THH, THT, TTH, TTT}.
    - Event: Getting exactly two heads, E = {HHT, HTH, THH}.



---


## 2. Types of Probability

Probability can be interpreted and calculated in different ways depending on the context and available information. The three main types are:

### 1. Theoretical (Classical) Probability
This approach is based on mathematical reasoning and assumes all outcomes are equally likely. It is used when the structure of the experiment is well-defined and all possible outcomes can be listed.

**Formula:**  
\( P(E) = \frac{\text{Number of favorable outcomes}}{\text{Total number of possible outcomes}} \)

**Example:**  
- Rolling a fair six-sided die:  
    There are 6 possible outcomes (1, 2, 3, 4, 5, 6).  
    Probability of rolling a 3:  
    \( P(3) = \frac{1}{6} \)

**Use Cases:**  
- Card games, dice rolls, lotteries, and other games of chance.

**Example:**  
Suppose you want to find the probability of drawing a heart from a standard deck of 52 playing cards.

- **Number of favorable outcomes:** 13 (since there are 13 hearts in the deck)
- **Total number of possible outcomes:** 52

**Classical Probability Formula:**  
\( P(\text{Heart}) = \frac{13}{52} = 0.25 \)


### 2. Experimental (Empirical) Probability
This type is based on actual data from experiments or observations. It is calculated by performing an experiment multiple times and recording the frequency of each outcome.

**Useful when outcomes are not equally likely:**  
Experimental probability is especially valuable when the possible outcomes of an experiment do not have the same chance of occurring, or when the theoretical model is unknown or complex. By observing real-world frequencies, you can estimate probabilities even if the outcomes are not equally likely.

**Example:**  
Suppose you want to know the probability that a bus arrives late at your stop. The bus schedule is complex, and you don’t know the exact odds. So, you record what happens for 30 days:

- The bus is late on 9 days.
- The bus is on time on 21 days.

Experimental probability of the bus being late:
- Number of times late ÷ Total number of days = 9 ÷ 30 = 0.3 (or 30%)

Here, you used real-world data (not theory) to estimate the probability. The outcomes (late/on time) are not guaranteed to be equally likely, and you didn’t need to know the underlying model—just your observations.

**Formula:**  
\( P(E) = \frac{\text{Number of times event E occurs}}{\text{Total number of trials}} \)

**How It Works:**  
- Conduct the experiment or observe the process repeatedly.
- Count how many times the event of interest occurs.
- Divide by the total number of trials to estimate the probability.

**Example:**  
- Flipping a coin 100 times and getting 56 heads:  
    Empirical probability of heads = \( \frac{56}{100} = 0.56 \)
- Rolling a die 60 times and getting a 4 twelve times:  
    Empirical probability of rolling a 4 = \( \frac{12}{60} = 0.2 \)

**Additional Examples:**  
- Surveying 200 people and finding that 120 prefer tea:  
    Empirical probability someone prefers tea = \( \frac{120}{200} = 0.6 \)
- Observing 50 cars at an intersection and 15 run a red light:  
    Empirical probability a car runs a red light = \( \frac{15}{50} = 0.3 \)
- Testing 80 manufactured items and 5 are defective:  
    Empirical probability an item is defective = \( \frac{5}{80} = 0.0625 \)

**Key Points:**  
- Empirical probability reflects observed outcomes, not theoretical expectations.
- Results may vary from theoretical probability due to randomness or small sample sizes.
- As the number of trials increases, empirical probability tends to approach theoretical probability (Law of Large Numbers).

**Applications:**  
- Used in scientific experiments, surveys, market research, and quality control.
- Helps estimate probabilities when theoretical models are unavailable or complex.
- Useful for validating theoretical predictions with real-world data.
- Can reveal unexpected patterns or biases in experiments.

**Limitations:**  
- Requires sufficient data for reliable estimates.
- May be affected by experimental errors or sampling bias.
- Not always generalizable beyond the observed trials.

**Use Cases:**  
- Scientific experiments, surveys, quality control, and any situation where outcomes are observed and counted.

**Note:**  
Empirical probability may differ from theoretical probability due to randomness or limited sample size, but it tends to approach the theoretical value as the number of trials increases (Law of Large Numbers).

### 3. Subjective Probability
This is based on personal judgment, intuition, or experience rather than formal calculations or data. It is often used when there is incomplete information or when outcomes cannot be measured precisely.

**Example:**  
- Estimating a 60% chance of rain tomorrow based on your experience and current weather conditions, even without meteorological data.
- A doctor’s belief that a patient has a 90% chance of recovery based on their expertise and past cases.

**Use Cases:**  
- Decision making under uncertainty, expert opinions, forecasting, and risk assessment.

**Note:**  
Subjective probability is influenced by individual beliefs and may vary from person to person.

---

**Summary Table:**

| Type           | Basis                | Calculation Method                | Example                        |
|----------------|---------------------|-----------------------------------|--------------------------------|
| Theoretical    | Mathematical model  | Count favorable/total outcomes    | Dice, cards, coins             |
| Experimental   | Observed data       | Frequency in repeated trials      | Coin flips, surveys            |
| Subjective     | Personal judgment   | Intuition, experience             | Weather forecasts, expert opinion |

## 3. Real-Life Relevance of Probability



Probability is widely used in various fields to make informed decisions and predictions. Here are some practical examples:

- **Medical Trials:**  
    Probability helps assess the effectiveness of new drugs. For instance, if a clinical trial finds that 80 out of 100 patients recover after taking a medication, the empirical probability of recovery is 0.8 (or 80%).  
    Another example: In vaccine studies, if 950 out of 1,000 vaccinated individuals do not contract the disease, the probability of immunity is 0.95 (or 95%).  
    Probability is also used to estimate the likelihood of side effects, predict disease outbreaks, and evaluate diagnostic test accuracy.

- **Insurance:**  
    Insurers use probability to estimate the risk of claims. For example, if historical data shows that 1 in 50 policyholders file a claim each year, the probability of a claim is 0.02 (or 2%).  
    Another example: Life insurance companies calculate the probability of payout based on age and health statistics, such as a 0.005 (0.5%) annual probability of payout for a healthy 30-year-old.  
    Probability models also help set premiums, forecast losses, and manage risk for natural disasters or accidents.

- **Business:**  
    Companies use probability to forecast sales and optimize inventory. If a store observes that 60% of customers buy a particular product, it can use this probability to plan stock levels and avoid shortages.  
    Another example: An online retailer estimates a 30% probability that a visitor will make a purchase, helping set marketing budgets and predict revenue.  
    Businesses also use probability to assess project risks, analyze customer behavior, and make investment decisions.

- **Games:**  
    Probability determines fairness and expected winnings in games of chance. For example, in a dice game where rolling a six wins $10, the probability of winning is 1/6. The expected winnings per roll are \( \frac{1}{6} \times \$10 = \$1.67 \).  
    Another example: In a card game, the probability of drawing a heart from a standard deck is 13/52 (or 25%), which can be used to calculate expected returns or odds.  
    Probability is also used in sports betting, lotteries, and casino games to set odds and payouts.

- **Weather Forecasting:**  
    Meteorologists use probability to predict the chance of rain, snow, or storms. For example, a 70% chance of rain means that in similar conditions, rain occurred 70% of the time.

- **Engineering and Reliability:**  
    Engineers use probability to estimate the likelihood of system failures, product defects, or maintenance needs. For example, the probability that a machine will fail within a year might be 0.1 (10%).

- **Technology and Machine Learning:**  
    Probability underpins algorithms for spam detection, recommendation systems, and predictive analytics. For example, a spam filter might assign a 95% probability that an email is spam based on its content.

- **Finance:**  
    Probability is used to assess investment risks, price options, and forecast market trends. For example, the probability of a stock price rising above a certain level can inform trading strategies.

- **Quality Control:**  
    Manufacturers use probability to estimate the proportion of defective products and improve production processes. For example, if 3 out of 100 items are defective, the probability of picking a defective item is 0.03 (3%).

- **Epidemiology:**  
    Probability models help predict the spread of diseases, estimate infection rates, and evaluate the effectiveness of interventions.

These examples show how probability helps quantify uncertainty, guide decision-making, and optimize outcomes in diverse real-world scenarios.

---

## 4. Key Properties of Probability (Fundamental Laws)





a. **Range:**  
\( 0 \leq P(E) \leq 1 \)  
Probability can never be negative or greater than 1.

b. **Sum Rule:**  
The total probability of the sample space (all possible outcomes) is 1.  
\( P(S) = 1 \)

The Sum Rule in probability states that the probability of all possible outcomes (the sample space) adds up to 1. This means something in the sample space must happen.

**Example:**  
Suppose you roll a fair six-sided die. The sample space is {1, 2, 3, 4, 5, 6}.  
Each outcome has probability \( \frac{1}{6} \).

**Sum of probabilities:**  
\( P(1) + P(2) + P(3) + P(4) + P(5) + P(6) = \frac{1}{6} \times 6 = 1 \)

**Key Point:**  
No matter what, one of the outcomes will occur, so the total probability is always 1.


c. **Complement Rule:**  
The probability of an event not happening is:  
\( P(\text{Not } A) = 1 - P(A) \)

**Example:**  
If the probability of rain tomorrow is 0.3, then the probability it does not rain is:  
\( P(\text{No Rain}) = 1 - 0.3 = 0.7 \)

---

d. **Addition Rule (Mutually Exclusive Events):**  
For events that cannot happen at the same time:  
\( P(A \cup B) = P(A) + P(B) \)


Mutually Exclusive Events
Mutually exclusive events are events that cannot happen at the same time. In probability, if one event occurs, the other cannot. For example, when flipping a coin, getting "heads" and getting "tails" are mutually exclusive—only one outcome is possible per flip.

**Example:**  
If the probability of rolling a 2 on a die is 1/6 and rolling a 5 is 1/6, then:  
\( P(2 \text{ or } 5) = 1/6 + 1/6 = 2/6 = 1/3 \)

---

e. **General Addition Rule (Non-Mutually Exclusive Events):**  
For events that can overlap:  
\( P(A \cup B) = P(A) + P(B) - P(A \cap B) \)

Key Points:

If events A and B are mutually exclusive, then P(A and B) = 0.
The probability that either event A or event B occurs is:
P(A or B) = P(A) + P(B)

**Example:**  
In a class, 40% play soccer, 30% play basketball, and 10% play both.  
\( P(\text{Soccer or Basketball}) = 0.4 + 0.3 - 0.1 = 0.6 \)

---

f. **Multiplication Rule (Independent Events):**  
For events that do not affect each other (i.e., the occurrence of one event does not change the probability of the other):  
\( P(A \cap B) = P(A) \cdot P(B) \)

**Independent Events Explained:**  
Two events are independent if knowing the outcome of one event gives no information about the outcome of the other. In other words, the probability of both events happening together is simply the product of their individual probabilities.

**Examples of Independent Events:**  
- Flipping a coin and rolling a die: The result of the coin flip does not influence the die roll.
- Drawing a card from one deck and rolling a die: The card drawn does not affect the die outcome.
- Tossing two coins: The result of the first toss does not affect the second.

**Example Calculation:**  
If the probability of flipping heads on a coin is 0.5 and rolling a 4 on a die is 1/6, then:  
\( P(\text{Heads and 4}) = 0.5 \times \frac{1}{6} = 0.083 \)

**Key Point:**  
If events are not independent (i.e., the outcome of one affects the other), you must use conditional probability instead:  
\( P(A \cap B) = P(A) \times P(B|A) \)




## 5. More Real-World Examples & Applications


### Probability

1. **Weather Forecasting**  
    Meteorologists use historical data and statistical models to predict the likelihood of weather events.  
    *Example:* "There's a 70% chance of rain tomorrow" means that, based on similar past conditions, rain occurred 70% of the time.
    *Example:* Predicting the probability of a hurricane making landfall in a given region during a season.
    *Example:* Estimating the chance of snowfall on a specific day based on climate data.

2. **Medical Testing**  
    Doctors use probability to interpret test results, considering disease prevalence and test accuracy (sensitivity and specificity).  
    *Example:* If a disease affects 1% of people and a test is 99% accurate, probability helps estimate the chance a person actually has the disease after a positive result (using Bayes' theorem).
    *Example:* Calculating the probability of a false positive or false negative result in cancer screening.
    *Example:* Assessing the likelihood of side effects from a new medication in clinical trials.

3. **Insurance Industry**  
    Insurance companies assess risk and set premiums using probability models.  
    *Example:* Calculating the probability of a car accident based on age and driving history helps determine insurance rates.
    *Example:* Estimating the probability of a house fire to set homeowner insurance premiums.
    *Example:* Determining life insurance rates based on the probability of certain health events.

4. **Quality Control in Manufacturing**  
    Manufacturers use probability to determine acceptable defect rates and optimize production.  
    *Example:* Using sampling methods to estimate the probability of defects in a batch of 10,000 microchips based on testing just 100 units.
    *Example:* Calculating the probability that a randomly selected product meets quality standards.
    *Example:* Estimating the likelihood of a machine breakdown based on historical failure rates.

5. **Stock Market Analysis**  
    Investors use probability models to assess investment risks and potential returns.  
    *Example:* Calculating the probability that a stock will increase in value by 10% within six months based on historical performance data.
    *Example:* Estimating the likelihood of a market crash using statistical models.
    *Example:* Assessing the probability of achieving a target return in a diversified portfolio.

---

## 6. Permutations

### What is a Permutation?
A **permutation** is an arrangement of objects in a specific order. In permutations, the order of selection is important. Permutations are used when you are selecting and arranging elements from a set, and each arrangement is considered unique if the order is different.

**Key Points:**
- Order matters.
- No element is used more than once (unless stated otherwise).
- Used for arrangements, rankings, seatings, etc.

### Permutation Formula

If you have \( n \) distinct objects and want to arrange \( r \) of them in order, the number of permutations is:

\[
P(n, r) = \frac{n!}{(n - r)!}
\]

Where:
- \( n! \) (n factorial) is the product of all positive integers up to \( n \).
- \( r \) is the number of objects to arrange.

---

### Real-Life Examples

#### 1. Password Generation

**Problem:**  
How many 4-digit PIN codes can be formed using the digits 0–9, with no repetition?

**Solution:**  
- There are 10 digits (0–9).
- We need to arrange 4 digits, and order matters (e.g., 1234 ≠ 4321).
- No digit repeats.

\[
P(10, 4) = \frac{10!}{(10-4)!} = \frac{10 \times 9 \times 8 \times 7 \times 6!}{6!} = 10 \times 9 \times 8 \times 7 = 5040
\]

**Answer:**  
There are **5,040** possible 4-digit PIN codes with no repeated digits.

---

#### 2. Seating Arrangement

**Problem:**  
In how many ways can 5 people be seated in 3 chairs?

**Solution:**  
- 5 people to choose from.
- 3 chairs to fill, and order matters (seat 1, seat 2, seat 3).
- No person sits in more than one chair.

\[
P(5, 3) = \frac{5!}{(5-3)!} = \frac{5 \times 4 \times 3 \times 2!}{2!} = 5 \times 4 \times 3 = 60
\]

**Answer:**  
There are **60** possible ways to seat 5 people in 3 chairs.

---

#### 3. Word Formation

**Problem:**  
How many different words can you form using the letters of “MATH”?

**Solution:**  
- There are 4 distinct letters: M, A, T, H.
- We want to arrange all 4 letters (order matters).

\[
P(4, 4) = 4! = 4 \times 3 \times 2 \times 1 = 24
\]

**Answer:**  
There are **24** different words (arrangements) that can be formed using all the letters of "MATH".

---

### More Permutation Examples

- **Arranging Books:**  
    How many ways can 6 different books be arranged on a shelf?  
    \( P(6, 6) = 6! = 720 \) ways.

- **Assigning Medals:**  
    In a race with 8 runners, how many ways can gold, silver, and bronze medals be awarded?  
    \( P(8, 3) = 8 \times 7 \times 6 = 336 \) ways.

---

### Summary Table

| Scenario                  | n (total items) | r (chosen) | Formula           | Result |
|---------------------------|-----------------|------------|-------------------|--------|
| 4-digit PIN (0–9, no rep) | 10              | 4          | \( P(10, 4) \)    | 5040   |
| 5 people, 3 chairs        | 5               | 3          | \( P(5, 3) \)     | 60     |
| 6 books, all arranged     | 6               | 6          | \( P(6, 6) \)     | 720    |
| 8 runners, 3 medals       | 8               | 3          | \( P(8, 3) \)     | 336    |
| "MATH" word formation     | 4               | 4          | \( P(4, 4) \)     | 24     |

---

### Important Concepts

- **Permutation vs. Combination:**  
    - **Permutation:** Order matters (e.g., 123 ≠ 321)
    - **Combination:** Order doesn’t matter (e.g., 123 = 321)

    - **Circular Permutation:**  
        - Used when elements are arranged in a circle.
        - Formula for \( n \) distinct objects: \( (n-1)! \)
        - **Example 1:**  
            How many ways can 5 people sit around a round table?  
            Solution: \( (5-1)! = 4! = 24 \) ways.
        - **Example 2:**  
            In how many ways can 7 different beads be arranged to form a circular bracelet?  
            Solution: \( (7-1)! = 6! = 720 \) ways.
        - **Example 3:**  
            Four friends want to play a board game that requires them to sit in a circle. How many different seating arrangements are possible?  
            Solution: \( (4-1)! = 3! = 6 \) ways.

    - **Special Case – All elements are used:**  
        - If we use all \( n \) elements (\( r = n \)): \( n! \) permutations
        - **Example 1:**  
            How many ways can 6 books be arranged on a shelf?  
            Solution: \( 6! = 720 \) ways.
        - **Example 2:**  
            How many ways can 5 runners line up for a photo?  
            Solution: \( 5! = 120 \) ways.
        - **Example 3:**  
            How many different ways can the letters of the word "PROB" be arranged?  
            Solution: There are 4 letters, so \( 4! = 24 \) ways.

    **More Clarifying Examples:**

    - **Example – Arranging People in a Row vs. Circle:**  
        - 4 people in a row: \( 4! = 24 \) ways.
        - 4 people in a circle: \( (4-1)! = 3! = 6 \) ways.

    - **Example – Circular Permutation with Identical Objects:**  
        - If some objects are identical, divide by the factorial of the number of identical objects.
        - For example, arranging 3 red and 2 blue beads in a circle:  
          Total arrangements = \( \frac{(5-1)!}{3! \times 2!} = \frac{24}{6 \times 2} = 2 \) ways.

    **Tip:**  
    - For circular permutations, fixing one position (to break rotational symmetry) avoids counting identical arrangements multiple times.
    - For linear permutations, every arrangement is unique because the start and end are fixed.


**Tip:**  
Use permutations when the arrangement or order of selection is important. If order does not matter, use combinations (covered in the next section).

## 7. Combinations

### What is a Combination?
A **combination** is a way of selecting items from a larger set where the order of selection does **not** matter. Unlike permutations, combinations focus only on which objects are chosen, not how they are arranged. Combinations are commonly used when forming groups, teams, or selecting items where arrangement is irrelevant.

**Key Points:**
- Order does **not** matter.
- No item is used more than once (unless stated otherwise).
- Used for group selections, committees, lottery draws, etc.

### Combination Formula

If you have \( n \) distinct objects and want to select \( r \) of them (order doesn't matter), the number of combinations is:

\[
C(n, r) = \binom{n}{r} = \frac{n!}{r!(n - r)!}
\]

Where:
- \( n! \) is the factorial of \( n \).
- \( r \) is the number of objects to select.

---

### Visualization Example

Imagine you have 4 colored balls: Red, Blue, Green, Yellow.  
If you select any 2 balls:

- Possible pairs:  
    - Red & Blue  
    - Red & Green  
    - Red & Yellow  
    - Blue & Green  
    - Blue & Yellow  
    - Green & Yellow

Notice:  
- Red & Blue is the **same** as Blue & Red (order doesn't matter).
- Total combinations: \( C(4, 2) = 6 \).

---

### Detailed Examples

#### 1. Forming a Committee

**Problem:**  
From a group of 7 people, how many ways can you select a committee of 3?

**Solution:**  
- Order doesn't matter (committee members are not ranked).
- Use the combination formula:

\[
C(7, 3) = \frac{7!}{3! \times 4!} = \frac{7 \times 6 \times 5}{3 \times 2 \times 1} = 35
\]

**Answer:**  
There are **35** ways to select a committee of 3 from 7 people.

---

#### 2. Lottery Selection

**Problem:**  
A lottery requires you to pick 6 numbers from 49. How many possible combinations are there?

**Solution:**  
- Order doesn't matter (6 numbers drawn, any order).
- Use the combination formula:

\[
C(49, 6) = \frac{49!}{6! \times 43!} = 13,983,816
\]

**Answer:**  
There are **13,983,816** possible combinations.

---

#### 3. Choosing Toppings

**Problem:**  
You can choose 2 toppings for your pizza from 5 options. How many different topping combinations can you have?

**Solution:**  
\[
C(5, 2) = \frac{5!}{2! \times 3!} = \frac{5 \times 4}{2 \times 1} = 10
\]

**Answer:**  
There are **10** possible topping combinations.

---

### Permutation vs. Combination: Quick Tip

Always ask:  
- **Does the order of selection matter?**
    - ✔ **Yes** → Use permutation
    - ✖ **No** → Use combination

---

### Summary Table

| Scenario                        | n (total items) | r (chosen) | Formula           | Result      |
|----------------------------------|-----------------|------------|-------------------|-------------|
| 4 balls, pick 2                 | 4               | 2          | \( C(4, 2) \)     | 6           |
| 7 people, committee of 3         | 7               | 3          | \( C(7, 3) \)     | 35          |
| 49 lottery numbers, pick 6      | 49              | 6          | \( C(49, 6) \)    | 13,983,816  |
| 5 pizza toppings, pick 2        | 5               | 2          | \( C(5, 2) \)     | 10          |

---

**Tip:**  
Use combinations when the arrangement of selected items is irrelevant. If arrangement matters, use permutations.

## 8. Detailed Explanation: Events in Probability

### What is an Event?
An **event** is a specific outcome or a set of outcomes from a random experiment. Events are fundamental to probability theory, as they represent the situations whose likelihood we want to measure.

**Examples:**
- Tossing a coin: Getting a Head is an event.
- Rolling a die: Getting an even number is an event.

---

### Types of Events with Examples

#### 1. Simple Event (Elementary Event)
A simple event involves only **one outcome** from the sample space.

- **Example 1:**  
    Rolling a die and getting a 3:  
    Event = {3}
- **Example 2:**  
    Drawing a card from a deck and getting the Ace of Spades:  
    Event = {Ace of Spades}
- **Example 3:**  
    Tossing a coin and getting Heads:  
    Event = {Heads}

#### 2. Compound Event
A compound event involves **two or more outcomes** from the sample space.

- **Example 1:**  
    Rolling a die and getting an odd number:  
    Event = {1, 3, 5}
- **Example 2:**  
    Drawing a card and getting a face card (Jack, Queen, King):  
    Event = {Jack, Queen, King of all suits}
- **Example 3:**  
    Tossing two coins and getting at least one Head:  
    Event = {HT, TH, HH}

#### 3. Certain Event
A certain event is **guaranteed to happen**; it includes all possible outcomes.

- **Example 1:**  
    Rolling a standard die and getting a number less than 7:  
    Event = {1, 2, 3, 4, 5, 6}  
    Probability = 1
- **Example 2:**  
    Drawing a card from a standard deck and getting a card between Ace and King:  
    Event = all 52 cards  
    Probability = 1
- **Example 3:**  
    Tossing a coin and getting either Heads or Tails:  
    Event = {Heads, Tails}  
    Probability = 1

#### 4. Impossible Event
An impossible event **cannot occur**; it contains no outcomes.

- **Example 1:**  
    Rolling a standard die and getting an 8:  
    Probability = 0
- **Example 2:**  
    Drawing a card from a standard deck and getting a card labeled "15":  
    Probability = 0
- **Example 3:**  
    Tossing a coin and getting both Heads and Tails at the same time:  
    Probability = 0

#### 5. Mutually Exclusive Events
Two events are **mutually exclusive** if they cannot occur at the same time.

- **Example 1:**  
    Tossing a coin: Getting a Head and a Tail in the same toss are mutually exclusive.
- **Example 2:**  
    Rolling a die: Getting a 2 and getting a 5 in one roll are mutually exclusive.
- **Example 3:**  
    Drawing a card: Drawing a Heart and a Club in a single draw are mutually exclusive.
- **Rule:**  
    If A and B are mutually exclusive:  
    \( P(A \cap B) = 0 \)

#### 6. Exhaustive Events
A set of events is **exhaustive** if it covers all possible outcomes of the experiment.

- **Example 1:**  
    Tossing a coin: Events {Head, Tail} are exhaustive.  
    \( P(\text{Head}) + P(\text{Tail}) = 1 \)
- **Example 2:**  
    Rolling a die: Events {1}, {2}, {3}, {4}, {5}, {6} are exhaustive.
- **Example 3:**  
    Drawing a card: Events {Red card}, {Black card} are exhaustive.

#### 7. Independent Events
Two events are **independent** if the occurrence of one does not affect the probability of the other.

- **Example 1:**  
    Tossing two coins:  
    - Event A: First coin is Head  
    - Event B: Second coin is Tail  
    A and B are independent.
- **Example 2:**  
    Rolling a die and tossing a coin:  
    - Event A: Die shows 4  
    - Event B: Coin shows Heads  
    These events are independent.
- **Example 3:**  
    Drawing a card from one deck and rolling a die:  
    The outcome of the card draw does not affect the die roll.
- **Rule:**  
    \( P(A \cap B) = P(A) \cdot P(B) \)

#### 8. Dependent Events
Events are **dependent** if the outcome of one affects the probability of the other.

- **Example 1:**  
    Drawing two cards from a deck without replacement:  
    - Event A: First card is a King  
    - Event B: Second card is also a King  
    The probability of B depends on the outcome of A.
- **Example 2:**  
    Picking two marbles from a bag without replacement:  
    - Event A: First marble is red  
    - Event B: Second marble is blue  
    The probability of B changes after A.
- **Example 3:**  
    Selecting students for two prizes from a class without replacement.

#### 9. Complementary Events
The **complement** of event A (written as \( A' \)) is the event that A does **not** happen.

- **Example 1:**  
    Event A: Rolling a die and getting a 6  
    Event A': Not getting a 6 (i.e., getting 1, 2, 3, 4, or 5)
- **Example 2:**  
    Event A: Drawing a red card from a deck  
    Event A': Drawing a black card
- **Example 3:**  
    Event A: It rains tomorrow  
    Event A': It does not rain tomorrow
- **Rule:**  
    \( P(A) + P(A') = 1 \)  
    or  
    \( P(A') = 1 - P(A) \)

---

### Summary Table: Types of Events

| Event Type             | Description                                      | Example                                      | Key Rule/Formula                |
|------------------------|--------------------------------------------------|----------------------------------------------|----------------------------------|
| Simple Event           | Single outcome                                   | Rolling a 3: {3}                             |                                  |
| Compound Event         | Multiple outcomes                                | Odd number on die: {1, 3, 5}                 |                                  |
| Certain Event          | Always occurs                                    | Number < 7 on die: {1,2,3,4,5,6}             | \( P = 1 \)                      |
| Impossible Event       | Never occurs                                     | Rolling an 8 on a die                        | \( P = 0 \)                      |
| Mutually Exclusive     | Cannot occur together                            | Head and Tail in one coin toss               | \( P(A \cap B) = 0 \)            |
| Exhaustive Events      | Cover all possible outcomes                      | {Head, Tail} in coin toss                    | Sum of probabilities = 1         |
| Independent Events     | One does not affect the other                    | Two coin tosses                              | \( P(A \cap B) = P(A)P(B) \)     |
| Dependent Events       | One affects the probability of the other         | Drawing cards without replacement            |                                  |
| Complementary Events   | Event and its complement cover all possibilities | Getting a 6 or not getting a 6 on a die      | \( P(A) + P(A') = 1 \)           |



**Tip:**  
Understanding the types of events and their relationships is crucial for solving probability problems accurately.

---

## 9. Examination Practice Problems

### Problem 1 (Easy): Basic Probability
A standard deck of 52 cards contains 13 hearts. What is the probability of drawing a heart from the deck?

**Solution:**
- Favorable outcomes = 13 (hearts)
- Total outcomes = 52 (total cards)
- P(Heart) = 13/52 = 1/4 = 0.25 or 25%

**Answer: 1/4 or 0.25 or 25%**

---

### Problem 2 (Easy): Complement Rule
If the probability of rain tomorrow is 0.35, what is the probability that it will NOT rain?

**Solution:**
- Using the complement rule: P(Not Rain) = 1 - P(Rain)
- P(Not Rain) = 1 - 0.35 = 0.65

**Answer: 0.65 or 65%**

---

### Problem 3 (Medium): Addition Rule with Mutually Exclusive Events
A die is rolled once. What is the probability of getting either a 2 or a 5?

**Solution:**
- Getting a 2 and getting a 5 are mutually exclusive events
- P(2) = 1/6, P(5) = 1/6
- P(2 or 5) = P(2) + P(5) = 1/6 + 1/6 = 2/6 = 1/3

**Answer: 1/3 ≈ 0.333 or 33.3%**

---

### Problem 4 (Medium): Independent Events
Two coins are tossed simultaneously. What is the probability of getting heads on both coins?

**Solution:**
- The coins are independent events
- P(Head on first coin) = 1/2
- P(Head on second coin) = 1/2
- P(Both heads) = P(Head) × P(Head) = 1/2 × 1/2 = 1/4

**Answer: 1/4 = 0.25 or 25%**

---

### Problem 5 (Medium): Conditional Probability
In a class of 30 students, 18 study Math, 12 study Physics, and 8 study both subjects. If a student is randomly selected and is found to study Math, what is the probability that they also study Physics?

**Solution:**
- Let M = studies Math, P = studies Physics
- P(M) = 18/30, P(P) = 12/30, P(M ∩ P) = 8/30
- P(P|M) = P(M ∩ P) / P(M) = (8/30) / (18/30) = 8/18 = 4/9

**Answer: 4/9 ≈ 0.444 or 44.4%**

---

### Problem 6 (Medium): Permutations
In how many ways can 4 people be arranged in a row for a photograph?

**Solution:**
- This is a permutation problem where order matters
- All 4 people are being arranged, so we use P(4,4) = 4!
- 4! = 4 × 3 × 2 × 1 = 24

**Answer: 24 ways**

---

### Problem 7 (Hard): Combinations with Multiple Selections
A committee of 5 people is to be formed from a group of 8 men and 6 women. In how many ways can the committee be formed if it must contain exactly 3 men and 2 women?

**Solution:**
- Ways to choose 3 men from 8: C(8,3) = 8!/(3!×5!) = 56
- Ways to choose 2 women from 6: C(6,2) = 6!/(2!×4!) = 15
- Total ways = C(8,3) × C(6,2) = 56 × 15 = 840

**Answer: 840 ways**

---

### Problem 8 (Hard): Bayes' Theorem
A medical test for a disease is 95% accurate for people who have the disease (sensitivity) and 90% accurate for people who don't have the disease (specificity). If 2% of the population has the disease, what is the probability that a person who tests positive actually has the disease?

**Solution:**
- Let D = has disease, T = tests positive
- P(D) = 0.02, P(D') = 0.98
- P(T|D) = 0.95, P(T|D') = 0.10
- P(T) = P(T|D)×P(D) + P(T|D')×P(D') = 0.95×0.02 + 0.10×0.98 = 0.019 + 0.098 = 0.117
- P(D|T) = P(T|D)×P(D) / P(T) = (0.95×0.02) / 0.117 = 0.019 / 0.117 ≈ 0.162

**Answer: ≈ 0.162 or 16.2%**

---

### Problem 9 (Hard): Dependent Events Without Replacement
A box contains 5 red balls and 3 blue balls. Two balls are drawn without replacement. What is the probability that both balls are red?

**Solution:**
- Total balls = 5 + 3 = 8
- P(First ball is red) = 5/8
- After removing one red ball: 4 red balls left, 7 total balls left
- P(Second ball is red | First ball is red) = 4/7
- P(Both red) = P(First red) × P(Second red | First red) = 5/8 × 4/7 = 20/56 = 5/14

**Answer: 5/14 ≈ 0.357 or 35.7%**

---

### Problem 10 (Very Hard): Complex Probability with Multiple Conditions
A factory produces items using three machines: A, B, and C. Machine A produces 30% of items with 2% defective rate, Machine B produces 45% of items with 3% defective rate, and Machine C produces 25% of items with 1% defective rate. If a randomly selected item is found to be defective, what is the probability it came from Machine B?

**Solution:**
- Let A, B, C = machines; D = defective item
- P(A) = 0.30, P(B) = 0.45, P(C) = 0.25
- P(D|A) = 0.02, P(D|B) = 0.03, P(D|C) = 0.01
- P(D) = P(D|A)×P(A) + P(D|B)×P(B) + P(D|C)×P(C)
- P(D) = 0.02×0.30 + 0.03×0.45 + 0.01×0.25 = 0.006 + 0.0135 + 0.0025 = 0.022
- P(B|D) = P(D|B)×P(B) / P(D) = (0.03×0.45) / 0.022 = 0.0135 / 0.022 ≈ 0.614

**Answer: ≈ 0.614 or 61.4%**

---

### Problem 11 (Easy): Basic Dice Probability
What is the probability of rolling a number greater than 4 on a standard six-sided die?

**Solution:**
- Sample space: {1, 2, 3, 4, 5, 6}
- Favorable outcomes: {5, 6} (numbers greater than 4)
- Number of favorable outcomes = 2
- Total outcomes = 6
- P(number > 4) = 2/6 = 1/3

**Answer: 1/3 ≈ 0.333 or 33.3%**

---

### Problem 12 (Easy): Simple Addition Rule
A bag contains 15 marbles: 6 red, 4 blue, and 5 green. What is the probability of drawing either a red or blue marble?

**Solution:**
- P(Red) = 6/15, P(Blue) = 4/15
- Red and Blue are mutually exclusive events
- P(Red or Blue) = P(Red) + P(Blue) = 6/15 + 4/15 = 10/15 = 2/3

**Answer: 2/3 ≈ 0.667 or 66.7%**

---

### Problem 13 (Medium): Experimental Probability
In 200 trials of flipping a biased coin, heads appeared 130 times. Based on this data, what is the experimental probability of getting heads? If the coin is flipped 50 more times, how many heads would you expect?

**Solution:**
- Experimental probability = Number of heads / Total trials
- P(Heads) = 130/200 = 0.65
- Expected heads in 50 trials = 0.65 × 50 = 32.5 ≈ 33 heads

**Answer: P(Heads) = 0.65 or 65%; Expected heads ≈ 33**

---

### Problem 14 (Medium): Circular Permutation
In how many ways can 6 people sit around a circular table?

**Solution:**
- For circular arrangements, we fix one position to avoid counting rotations
- Formula for circular permutation: (n-1)!
- Number of ways = (6-1)! = 5! = 5 × 4 × 3 × 2 × 1 = 120

**Answer: 120 ways**

---

### Problem 15 (Medium): General Addition Rule
In a survey of 100 students: 60 like pizza, 45 like burgers, and 25 like both. What is the probability that a randomly selected student likes either pizza or burgers?

**Solution:**
- P(Pizza) = 60/100 = 0.6
- P(Burger) = 45/100 = 0.45
- P(Both) = 25/100 = 0.25
- P(Pizza or Burger) = P(Pizza) + P(Burger) - P(Both)
- P(Pizza or Burger) = 0.6 + 0.45 - 0.25 = 0.8

**Answer: 0.8 or 80%**

---

### Problem 16 (Hard): Binomial Probability
A basketball player has a 75% free throw success rate. What is the probability of making exactly 3 out of 5 free throw attempts?

**Solution:**
- This is a binomial distribution: n = 5, k = 3, p = 0.75
- P(X = k) = C(n,k) × p^k × (1-p)^(n-k)
- P(X = 3) = C(5,3) × (0.75)³ × (0.25)²
- C(5,3) = 10, (0.75)³ = 0.4219, (0.25)² = 0.0625
- P(X = 3) = 10 × 0.4219 × 0.0625 = 0.2637

**Answer: ≈ 0.264 or 26.4%**

---

### Problem 17 (Hard): Complex Card Problem
From a standard deck of 52 cards, 3 cards are drawn without replacement. What is the probability that all 3 cards are aces?

**Solution:**
- There are 4 aces in the deck
- P(1st ace) = 4/52
- P(2nd ace | 1st ace) = 3/51
- P(3rd ace | 1st and 2nd aces) = 2/50
- P(All 3 aces) = (4/52) × (3/51) × (2/50) = 24/132,600 = 1/5,525

**Answer: 1/5,525 ≈ 0.000181 or 0.0181%**

---

### Problem 18 (Hard): Combination with Restrictions
A committee of 6 people must be selected from 10 men and 8 women. How many ways can this be done if the committee must have at least 2 women?

**Solution:**
- Total ways to select 6 from 18 people = C(18,6)
- Ways with 0 women = C(10,6) × C(8,0) = 210 × 1 = 210
- Ways with 1 woman = C(10,5) × C(8,1) = 252 × 8 = 2,016
- Ways with at least 2 women = C(18,6) - 210 - 2,016
- C(18,6) = 18,564
- Ways with at least 2 women = 18,564 - 210 - 2,016 = 16,338

**Answer: 16,338 ways**

---

### Problem 19 (Very Hard): Multi-Stage Probability
A company has three production lines. Line A produces 40% of products with 5% defect rate, Line B produces 35% with 3% defect rate, and Line C produces 25% with 7% defect rate. A quality inspector randomly selects a product and finds it defective. What is the probability it came from Line A? What if the inspector then selects another defective product independently?

**Solution:**
**Part 1:**
- P(A) = 0.4, P(B) = 0.35, P(C) = 0.25
- P(D|A) = 0.05, P(D|B) = 0.03, P(D|C) = 0.07
- P(D) = 0.05×0.4 + 0.03×0.35 + 0.07×0.25 = 0.02 + 0.0105 + 0.0175 = 0.048
- P(A|D) = (0.05×0.4)/0.048 = 0.02/0.048 = 5/12 ≈ 0.417

**Part 2:**
- Probability both defective products are from Line A = P(A|D)²
- P(Both from A) = (5/12)² = 25/144 ≈ 0.174

**Answer: Part 1: 5/12 ≈ 41.7%; Part 2: 25/144 ≈ 17.4%**

---

### Problem 20 (Very Hard): Advanced Conditional Probability
In a game, Player 1 wins 60% of the time against Player 2. They play a best-of-5 series (first to win 3 games). Given that Player 1 wins the series, what is the probability that the series went exactly 5 games (3-2 result)?

**Solution:**
- Let W = Player 1 wins series, F = series goes 5 games
- For series to go 5 games with P1 winning: P1 must win exactly 2 of first 4, then win game 5
- Ways to win 2 of first 4: C(4,2) = 6
- P(Win exactly 2 of 4) = C(4,2) × (0.6)² × (0.4)² = 6 × 0.36 × 0.16 = 0.3456
- P(Win game 5) = 0.6
- P(Win series in 5) = 0.3456 × 0.6 = 0.20736

- P(Win series overall) needs to be calculated:
  - Win in 3: (0.6)³ = 0.216
  - Win in 4: C(3,2) × (0.6)² × 0.4 × 0.6 = 3 × 0.36 × 0.4 × 0.6 = 0.2592
  - Win in 5: 0.20736
  - P(Win series) = 0.216 + 0.2592 + 0.20736 = 0.68256

- P(5 games | Win series) = P(Win in 5) / P(Win series) = 0.20736 / 0.68256 ≈ 0.304

**Answer: ≈ 0.304 or 30.4%**

---

**Updated Scoring Guide for Examination:**
- Problems 1-2, 11-12 (Easy): 5 points each
- Problems 3-6, 13-15 (Medium): 10 points each  
- Problems 7-9, 16-18 (Hard): 15 points each
- Problems 10, 19-20 (Very Hard): 20 points each
- **Total: 200 points**

**Time Allocation Suggestion:**
- Easy problems: 3-5 minutes each
- Medium problems: 8-12 minutes each
- Hard problems: 15-20 minutes each
- Very hard problem: 25-30 minutes

--- 

*This tutorial provides a comprehensive foundation in probability theory. Continue practicing with diverse problems to strengthen your understanding and application skills.*







