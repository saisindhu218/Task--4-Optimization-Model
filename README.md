# Task--4-Optimization-Model

*Company*   : CODTECH IT SOLUTIONS

*Name*      : Rachabattuni Sai Sindhu

*Intern ID* : CT06DG1263

*Domain*    : Data Science

*Duration*  : 6 Weeks

*Mentor*    : Neela Santosh

###

As part of my Data Science internship at CODTECH and as an MCA student who is still new to this domain, I got the chance to work on an exciting real-world problem — figuring out the most profitable way for a company to produce multiple products with limited resources. This was my **first experience with optimisation techniques**, and it gave me hands-on exposure to how companies can use data and logic to make smarter decisions.

The focus of this task was a classic **“Product Mix Problem”**, where a factory must decide how many units of Products A, B, and C to produce in a week. Each product consumes different resources like machine time, raw materials, and labor hours, and also brings in different profit. The goal was to maximize total profit while staying within the limits of resource availability and market demand.

Using Python and the PuLP library, I created a Linear Programming (LP) model to solve this challenge and documented everything in a Jupyter Notebook (`optimisation_task4.ipynb`). The entire process — from problem understanding to modelling, solving, and visualizing — was new to me, and it really helped me learn step by step.

## Problem Details

| Product | Machine Time (hrs/unit) | Raw Material (kg/unit) | Labor Hours (hrs/unit) | Profit (\$/unit) | Max Demand (units/week) |
| ------- | ----------------------- | ---------------------- | ---------------------- | ---------------- | ----------------------- |
| A       | 3                       | 1                      | 2                      | 12               | 40                      |
| B       | 2                       | 2                      | 3                      | 10               | 35                      |
| C       | 4                       | 1                      | 2                      | 15               | 30                      |

### Resource Constraints per Week:

* Machine Time: 200 hours
* Raw Material: 150 kg
* Labor: 180 hours

The objective was to figure out how many units of A, B, and C to produce so that **profit is maximized**, while still meeting the above constraints.


## How I Solved It

1. **Mathematical Modelling:**
   I used Linear Programming to form the problem. The decision variables were the number of units of each product. The objective function maximized profit, and the constraints ensured we didn’t exceed resource limits or demand.

**Linear Programming**
**Decision Variables:**
Let:
x_A = units of Product A to produce

x_B = units of Product B to produce

x_C = units of Product C to produce
(All variables are non-negative integers)

**Objective Function:**
Maximize Total Profit:
Z = 12x_A + 10x_B + 15x_C

**Constraints:**
Machine Time: 3x_A + 2x_B + 4x_C ≤ 200

Raw Material: 1x_A + 2x_B + 1x_C ≤ 150

Labor Hours: 2x_A + 3x_B + 2x_C ≤ 180

**Demand Limits:**
x_A ≤ 40

x_B ≤ 35

x_C ≤ 30

3. **Implementation in Python:**
   Using the PuLP library, I created and solved the model in Python. The Jupyter Notebook format helped me write explanations and results alongside the code. I also used matplotlib for visualization and pandas for cleaner data handling.

4. **Result Analysis:**
   After solving the model, I got the optimal production quantities and the maximum achievable profit. I also analyzed resource utilization, checked which constraints were tight (fully used), and even learned about shadow prices — a new but interesting concept!


## **What I Learned:**

As someone completely new to optimisation, this project taught me a lot:
* How to translate a real-world scenario into a mathematical model
* The importance of constraints and objective functions in decision-making
* How to use PuLP in Python for solving LP problems
* Understanding how shadow prices and slack resources can guide smart business investments
* How to present data and solutions clearly using Jupyter Notebook and charts
Most importantly, I learned that data science is not just about coding — it’s about solving real problems and delivering insights that matter.


## Conclusion

This project helped me experience what it’s like to solve business problems with data science tools. Even as a beginner, I was able to build something useful that can guide real production decisions. With the help of Python and LP modelling, a company can now decide how to produce efficiently, maximize profits, and plan better — instead of relying on guesswork.

Working on this task gave me confidence in approaching more advanced concepts in the future and showed me how data science can be a powerful decision-making tool in operations and resource management.

