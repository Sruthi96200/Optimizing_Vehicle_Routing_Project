📌 Project Title
Optimizing Vehicle Routing with Time Windows Using Julia

📖 Overview
This project addresses the Vehicle Routing Problem with Time Windows (VRPTW) — a classic logistics optimization challenge. A homogeneous fleet of vehicles must deliver to a set of customers, adhering to strict delivery time windows and vehicle capacity constraints. Each route starts and ends at a central depot. The primary objective is to minimize the total number of vehicles utilized, ensuring that:

Each customer is visited exactly once

Time window and capacity constraints are fully respected

⚙️ Methodology
1. Mixed-Integer Linear Programming (MILP)
A detailed MILP formulation is developed using the JuMP package in Julia. The model includes:

Binary decision variables to represent whether a vehicle travels from one node to another

Continuous variables to track service start times

Constraints for time windows, route flow, and capacity limitations

This model provides an exact solution to the VRPTW using a mathematical programming approach.

2. Column Generation Technique
To scale the problem efficiently, the project also implements a Column Generation approach:

Begins with a set of trivial routes (each serving a single customer)

Iteratively solves a restricted master problem

Uses a pricing subproblem to generate cost-reducing new routes

This decomposition method is especially effective for large-scale instances with many customers.

📊 Dataset & Assumptions
Customer coordinates and demand values are provided

Depot is defined as the final entry in the dataset

Travel times are computed using Euclidean distances

All inputs are assumed to be non-negative integers

💡 Key Highlights
Implemented in Julia using the JuMP optimization framework

Demonstrates both exact and scalable heuristic approaches

Includes code, visualizations, and performance comparisons

Applicable to real-world transportation, distribution, and supply chain scenarios

🔍 Skills Demonstrated
Combinatorial Optimization

Mathematical Modeling (MILP)

Column Generation & Decomposition Techniques

Algorithm Design in Julia

