# Advanced Probability Concepts

## Recap: Basic Probability Definitions

### Types of Probability
- **Classical Probability**: Based on equally likely outcomes (e.g., rolling a fair die).
- **Empirical Probability**: Based on observed data (e.g., probability it rains tomorrow based on past weather).
- **Subjective Probability**: Based on personal judgment or experience (e.g., a doctor's estimate of recovery chances).

### Events and Rules
- **Event**: A set of outcomes (e.g., getting heads in a coin toss).
- **Sample Space**: All possible outcomes (e.g., {Heads, Tails}).
- **Addition Rule**: For mutually exclusive events, P(A or B) = P(A) + P(B).
- **Multiplication Rule**: For independent events, P(A and B) = P(A) × P(B).

### Permutations & Combinations
- **Permutation**: Arrangements where order matters (e.g., arranging 3 books: 3! = 6 ways).
- **Combination**: Selections where order does not matter (e.g., choosing 2 out of 5 students: 5C2 = 10 ways).

---

## What is Joint Probability?

Joint Probability is the probability of two events occurring **together** at the same time.

**Examples:**
- What’s the probability that a student studies both Math and Science?
- What’s the probability it’s raining **and** cold today?

### Formal Definition
Joint probability of events A and B is written as:

    P(A ∩ B)

Pronounced as: “Probability of A **and** B happening.”

### Key Formulas
- For any two events A and B:
    - P(A ∩ B) = Probability that both A and B happen
- If A and B are **independent**:
    - P(A ∩ B) = P(A) × P(B)
- If A and B are **dependent**:
    - P(A ∩ B) = P(A|B) × P(B) = P(B|A) × P(A)

#### Example
In a class of 100 students:
- 60 students take Math → P(Math) = 0.60
- 40 students take Science → P(Science) = 0.40
- 25 students take both → P(Math ∩ Science) = 0.25

So, the probability that a randomly selected student takes both subjects is:

    P(Math ∩ Science) = 0.25 or 25%

#### Real-World Applications
- **Business**: P(Customer buys both Product A and Product B)
- **Weather**: P(It rains ∩ It is cold)
- **Healthcare**: P(Patient has a disease ∩ Test comes positive)
- **Marketing**: P(User opens email ∩ Clicks the link)

#### Demonstrative Example
**Q:** In a survey, 30% of people like tea, 20% like coffee, and 10% like both. What is the probability a person likes both tea and coffee?

**A:** P(Tea ∩ Coffee) = 0.10

**Q:** A survey of 100 students found that:

60 students like pizza
40 students like sushi
20 students like both pizza and sushi
What is the probability that a randomly selected student likes:

a) Pizza and sushi? b) Pizza or sushi? c) Neither pizza nor sushi?

**A:** a) P(Pizza and Sushi) = 20/100 = 0.2 b) P(Pizza or Sushi) = P(Pizza) + P(Sushi) - P(Pizza and Sushi) = 0.6 + 0.4 - 0.2 = 0.8 c) P(Neither Pizza nor Sushi) = 1 - P(Pizza or Sushi) = 1 - 0.8 = 0.2

**Q:**
A coin is tossed twice. Let A be the event that the first toss is heads, and B be the event that the second toss is tails.

a) What is P(A and B)? b) What is P(A or B)? c) Are A and B independent events?

**A:** a) P(A and B) = P(HT) = 1/4 = 0.25 b) P(A or B) = P(A) + P(B) - P(A and B) = 0.5 + 0.5 - 0.25 = 0.75 c) Yes, A and B are independent events because P(A and B) = P(A)P(B) = (0.5)(0.5) = 0.25

**Q:**
A deck of 52 cards is shuffled, and two cards are drawn at random. Let A be the event that the first card is a heart, and B be the event that the second card is a diamond.

a) What is P(A and B)? b) What is P(A or B)? c) Are A and B independent events?

**A:** a) P(A and B) = P(Heart and Diamond) = (13/52)(13/51) = 13/204 ≈ 0.0637 b) P(A or B) = P(A) + P(B) - P(A and B) = 0.25 + 0.25 - 0.0637 ≈ 0.4363 c) Yes, A and B are approximately independent events because the deck is large and the probability of drawing a heart and then a diamond is close to the product of the individual probabilities.

**Q:**
A factory produces two types of products, A and B. The probability that a product is of type A is 0.6, and the probability that a product is of type B is 0.4. The probability that a product is defective given that it is of type A is 0.1, and the probability that a product is defective given that it is of type B is 0.2.

a) What is the probability that a randomly selected product is defective and of type A? b) What is the probability that a randomly selected product is defective and of type B? c) What is the overall probability that a randomly selected product is defective?

**A:** a) P(Defective and A) = P(Defective|A)P(A) = (0.1)(0.6) = 0.06 b) P(Defective and B) = P(Defective|B)P(B) = (0.2)(0.4) = 0.08 c) P(Defective) = P(Defective and A) + P(Defective and B) = 0.06 + 0.08 = 0.14

**Q:**
A medical test has a 90% chance of detecting a disease if the patient has it (sensitivity), and a 10% chance of giving a false positive result if the patient does not have the disease (specificity). The prevalence of the disease in the population is 1%.

a) What is the probability that a patient tests positive and actually has the disease? b) What is the probability that a patient tests positive but does not have the disease? c) What is the overall probability that a patient tests positive?

**A:** a) P(Disease and Positive) = P(Positive|Disease)P(Disease) = (0.9)(0.01) = 0.009 b) P(No Disease and Positive) = P(Positive|No Disease)P(No Disease) = (0.1)(0.99) = 0.099 c) P(Positive) = P(Disease and Positive) + P(No Disease and Positive) = 0.009 + 0.099 = 0.108

**Q:**
Two events A and B have the following joint probability table:

B = 0	B = 1
A = 0	0.4	0.3
A = 1	0.2	0.1
a) What is P(A = 1 and B = 1)? b) What is P(A = 1 or B = 1)? c) Are A and B independent events?

**A:** a) P(A = 1 and B = 1) = 0.1 b) P(A = 1 or B = 1) = P(A = 1) + P(B = 1) - P(A = 1 and B = 1) = 0.3 + 0.4 - 0.1 = 0.6 c) No, A and B are not independent events because P(A = 1 and B = 1) ≠ P(A = 1)P(B = 1)

**Q:**
A box contains 5 red balls and 3 blue balls. Two balls are drawn at random without replacement. Let A be the event that the first ball is red, and B be the event that the second ball is blue.

a) What is P(A and B)? b) What is P(A or B)? c) Are A and B independent events?

**A:** a) P(A and B) = P(Red and Blue) = (5/8)(3/7) = 15/56 ≈ 0.2679 b) P(A or B) = P(A) + P(B) - P(A and B) = 5/8 + 3/8 - 15/56 ≈ 0.7857 c) No, A and B are not independent events because the probability of drawing a blue ball changes after drawing a red ball.

---

## Understanding Conditional Probability

Conditional Probability is the probability of an event occurring **given** that another event has already occurred.

    P(A | B) = Probability of A happening given B has happened

### Formal Definition
    P(A | B) = P(A ∩ B) / P(B),  provided that P(B) > 0

#### Example
100 students in a class:
- 60 passed Math → P(Math) = 0.60
- 40 passed both Math and Science → P(Math ∩ Science) = 0.40

What is the probability that a student passed Science, **given** they passed Math?

    P(Science | Math) = P(Math ∩ Science) / P(Math) = 0.40 / 0.60 = 0.6667 ≈ 66.7%

#### Real-Life Analogies
- **Medical Testing**: P(Has disease | Tested positive)
- **Weather**: P(Rains | It's cloudy)
- **Marketing**: P(Buys product | Opened email)

#### Demonstrative Example
**Q:** In a company, 70% of employees know Python, 50% know SQL, and 40% know both. What is the probability an employee knows SQL, given they know Python?

**A:**
P(SQL | Python) = P(Python ∩ SQL) / P(Python) = 0.40 / 0.70 ≈ 0.571 or 57.1%

---

## Independent Events

Two events A and B are **independent** if the occurrence of one does **not** affect the probability of the other.

### Mathematical Definition
- P(A ∩ B) = P(A) × P(B)
- P(A | B) = P(A)
- P(B | A) = P(B)

#### Example 1: Tossing Coins
Toss 2 fair coins:
- Event A: First coin is Heads → P(A) = ½
- Event B: Second coin is Tails → P(B) = ½
- P(A ∩ B) = ½ × ½ = ¼

#### Example 2: Rolling Dice
Roll two 6-sided dice:
- Event A: Die 1 shows a 3
- Event B: Die 2 shows an even number
- P(A ∩ B) = P(A) × P(B) = (1/6) × (3/6) = 1/12

#### How to Test Independence in Data
If P(A ∩ B) = P(A) × P(B), events are independent; else, they are dependent.

#### Real-World Independent Events
- Weather and outcome of a coin toss
- Rolling two different dice
- Choosing a card from a deck, replacing it, then choosing again
- Birthdays of two randomly chosen people

#### Demonstrative Example
**Q:** In a factory, 80% of machines are working, and 60% of workers are present. If these are independent, what is the probability a randomly chosen machine is working **and** a worker is present?

**A:**
P(Working ∩ Present) = 0.80 × 0.60 = 0.48 or 48%

---

## Bayes’ Theorem

Bayes’ Theorem allows us to **update our beliefs** about the likelihood of an event based on new evidence.

### Formula
    P(A | B) = [P(B | A) × P(A)] / P(B)

Where:
- P(A | B): Probability of A given B (what we want to find)
- P(B | A): Probability of B given A (what we know)
- P(A): Prior probability of A (initial belief)
- P(B): Total probability of B (evidence)

#### Step-by-Step Example
A rare disease affects 1% of the population. A test is:
- 99% accurate if the person has the disease → P(Positive | Disease) = 0.99
- 95% accurate if the person does NOT have the disease → P(Negative | No Disease) = 0.95 → P(Positive | No Disease) = 0.05

Known:
- P(Disease) = 0.01
- P(No Disease) = 0.99
- P(Positive | Disease) = 0.99
- P(Positive | No Disease) = 0.05

First, calculate P(Positive):
P(Positive) = [P(Positive | Disease) × P(Disease)] + [P(Positive | No Disease) × P(No Disease)]
           = (0.99 × 0.01) + (0.05 × 0.99)
           = 0.0099 + 0.0495 = 0.0594

Now apply Bayes’ Theorem:
P(Disease | Positive) = (0.99 × 0.01) / 0.0594 ≈ 0.1667 or 16.7%

#### Real-World Example
**Q:** A company launches a new product. 5% of customers are expected to buy it. If a customer clicks an ad, the probability they buy is 40%. If a customer does not buy, the probability they still click is 10%. What is the probability a customer buys, given they clicked?

**A:**
Let A = Buys, B = Clicks
- P(A) = 0.05
- P(B | A) = 0.40
- P(B | Not A) = 0.10
- P(Not A) = 0.95

P(B) = (0.40 × 0.05) + (0.10 × 0.95) = 0.02 + 0.095 = 0.115
P(A | B) = (0.40 × 0.05) / 0.115 ≈ 0.174 or 17.4%

---

## Summary
- **Joint Probability**: P(A ∩ B) — Probability of two events occurring together
- **Conditional Probability**: P(A|B) — Probability of A given B
- **Independence**: P(A ∩ B) = P(A)×P(B)
- **Bayes’ Theorem**: Inverts conditional probabilities to update beliefs

---

## Practice Questions & Answers

### 1. Joint Probability
**Q:** In a class, 70% like football, 50% like basketball, and 30% like both. What is the probability a student likes both?
**A:** P(Football ∩ Basketball) = 0.30

### 2. Conditional Probability
**Q:** In a survey, 40% own a car, 25% own both a car and a bike. What is the probability a person owns a bike, given they own a car?
**A:**
P(Bike | Car) = P(Car ∩ Bike) / P(Car) = 0.25 / 0.40 = 0.625 or 62.5%

### 3. Independence
**Q:** A die is rolled and a coin is tossed. What is the probability of getting a 4 and a head?
**A:**
P(4) = 1/6, P(Head) = 1/2
P(4 ∩ Head) = 1/6 × 1/2 = 1/12

### 4. Bayes’ Theorem
**Q:** 2% of emails are spam. A filter detects spam 95% of the time, but also flags 1% of non-spam as spam. What is the probability an email is spam, given it was flagged?
**A:**
Let S = Spam, F = Flagged
P(S) = 0.02, P(F|S) = 0.95, P(F|Not S) = 0.01, P(Not S) = 0.98
P(F) = (0.95 × 0.02) + (0.01 × 0.98) = 0.019 + 0.0098 = 0.0288
P(S|F) = (0.95 × 0.02) / 0.0288 ≈ 0.66 or 66%

---

## More Real-World Demonstrative Examples

### Example: Marketing
**Q:** 30% of users visit a website, 10% make a purchase, and 5% do both. What is the probability a user makes a purchase given they visited?
**A:**
P(Purchase | Visit) = P(Purchase ∩ Visit) / P(Visit) = 0.05 / 0.30 ≈ 0.167 or 16.7%

### Example: Healthcare
**Q:** 2% of people have a condition. A test detects it 90% of the time, but gives a false positive 8% of the time. What is the probability a person has the condition if they test positive?
**A:**
P(Condition) = 0.02, P(Pos|Cond) = 0.90, P(Pos|No Cond) = 0.08, P(No Cond) = 0.98
P(Pos) = (0.90 × 0.02) + (0.08 × 0.98) = 0.018 + 0.0784 = 0.0964
P(Cond|Pos) = (0.90 × 0.02) / 0.0964 ≈ 0.187 or 18.7%

---

**End of Notes**


