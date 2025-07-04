# Task-4--Optimization-Model

*Company*   : CODTECH IT SOLUTIONS

*Name*      : Rachabattuni Sai Sindhu

*Intern ID* : CT06DG1263

*Domain*    : Data Science

*Duration*  : 6 Weeks

*Mentor*    : Neela Santosh

###

As part of my Data Science internship at CODTECH and as an MCA student who is still new to this domain, I got the chance to work on an exciting real-world problem figuring out the most profitable way for a company to produce multiple products with limited resources. This was my **first experience with optimisation techniques**, and it gave me hands-on exposure to how companies can use data and logic to make smarter decisions.

The focus of this task was a classic **“Product Mix Problem”**, where a factory must decide how many units of Products A, B, and C to produce in a week. Each product consumes different resources like machine time, raw materials, and labor hours, and also brings in different profit. The goal was to maximize total profit while staying within the limits of resource availability and market demand.

Using Python and the PuLP library, I created a Linear Programming (LP) model to solve this challenge and documented everything in a Jupyter Notebook (optimisation_task4.ipynb). The entire process from problem understanding to modelling, solving, and visualizing was new to me, and it really helped me learn step by step.

## Project Workflow
### 1. Problem Details

| Product | Machine Time (hrs/unit) | Raw Material (kg/unit) | Labor Hours (hrs/unit) | Profit (\$/unit) | Max Demand (units/week) |
| ------- | ----------------------- | ---------------------- | ---------------------- | ---------------- | ----------------------- |
| A       | 3                       | 1                      | 2                      | 12               | 40                      |
| B       | 2                       | 2                      | 3                      | 10               | 35                      |
| C       | 4                       | 1                      | 2                      | 15               | 30                      |

#### Resource Constraints per Week:

* Machine Time: 200 hours
* Raw Material: 150 kg
* Labor: 180 hours

The objective was to figure out how many units of A, B, and C to produce so that **profit is maximized**, while still meeting the above constraints.


### 2. How I Solved It

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

### 3. **Implementation in Python:**

Using the PuLP library, I:

* Defined the LP problem and objective

* Added all constraints

* Set variable bounds

* Solved the model using PuLP’s built-in solver

This was done inside a Jupyter Notebook, which allowed me to document each step and see results interactively.


### 4. **Result Analysis:**
Once the model was solved:

* I retrieved the optimal values for x_A, x_B, and x_C

* Calculated the maximum profit

* Evaluated how much of each resource was used

* Identified binding constraints (fully used) and slack in others

* Explored shadow prices to understand how much additional profit could be earned by increasing resource availability

## **What I Learned**

As a beginner in data science and optimization, this project was a turning point in my learning journey. I understood how real-world business problems can be turned into mathematical models using Linear Programming (LP). I learned not just to code, but to think critically about constraints, decision variables, and resource limitations all from a problem-solving point of view.

Working with Python’s PuLP library helped me get comfortable formulating and solving optimization models. I discovered how shadow prices and slack values provide deep insight into which resources limit profit growth and which are underutilized. These concepts were completely new to me, but incredibly eye-opening.I also learned how to use Jupyter Notebooks to organize code, explanations, and visualizations neatly in one place. Creating visualizations helped me better communicate the results and understand the resource bottlenecks at a glance.

Most importantly, this task helped me realize that data science is not just about code it's about using logic, tools, and communication to drive meaningful business decisions.

### Key Takeaways:
* Translated a business scenario into a working mathematical model
* Built and solved an LP model using Python and PuLP
* Understood the role of objective functions and constraints in optimization
* Learned how to interpret shadow prices and slack for better decision-making
* Practiced clean documentation and clear explanations using Jupyter Notebook
* Used charts to visualize resource utilization and identify bottlenecks
* Gained confidence in applying data science to real-world problems


## Conclusion

This project gave me my first real experience in applying data science to solve a practical business problem. As a beginner, I was both excited and nervous to take on a task involving Python programming, linear programming, and mathematical modelling. But step by step, I learned how to approach the challenge from understanding the problem, writing the LP model, and implementing it using PuLP in Python, to interpreting the results and drawing meaningful business insights.

One of the biggest lessons I learned is that optimization is not just about math or coding it's about solving real-world problems in a smart and structured way. Through this project, I saw how companies can use data science tools to make better decisions, especially when resources are limited. Instead of guessing production levels, a factory can now rely on a model like this to produce efficiently, meet market demand, and maximize profits.I also discovered how powerful sensitivity analysis and shadow prices can be in understanding resource bottlenecks. These insights go beyond just solving for numbers they support strategic planning and help businesses see the value of investing in the right resources.

This task helped me grow more confident in working with Jupyter Notebooks, libraries like pandas and matplotlib, and visualizing data in a way that others can understand easily. It improved both my technical and communication skills, especially in presenting complex results in a clear and logical format.Overall, this project helped me experience what it’s like to solve business problems with data science tools. Even as a beginner, I was able to build something useful that can guide real production decisions. With the help of Python and LP modelling, a company can now decide how to produce efficiently, maximize profits, and plan better instead of relying on guesswork.Completing this project has motivated me to explore more in operations research, supply chain analytics, and optimization, and I’m excited to continue building my skills in this direction.

## Output
The Jupyter Notebook creation be like:
![Image](https://github.com/user-attachments/assets/67bd0b55-2645-49f4-abe0-298ec2a98fbe)

The optimization solution got excecuted
![Image](https://github.com/user-attachments/assets/e384a54e-4827-47f7-b068-b032346becab)

Visualization of the Resources we used
![Image](https://github.com/user-attachments/assets/154b4b83-3f87-49ca-a425-2e9666634df8)

