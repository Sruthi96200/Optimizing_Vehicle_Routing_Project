Optimizing Vehicle Routing with Time Windows Using Julia
This project focuses on solving the classical Vehicle Routing Problem with Time Windows (VRPTW), where a homogeneous fleet of vehicles must service a set of customers within specific time windows and capacity limits. Each route must begin and end at a central depot, and the objective is to minimize the total number of vehicles utilized, while ensuring that every customer is visited exactly once and within their designated time window.

To address this optimization challenge, the project implements two advanced methodologies:

1. Mixed-Integer Linear Programming (MILP):
A comprehensive MILP model is formulated by defining binary variables to represent vehicle routing decisions and continuous variables for service start times. The formulation incorporates essential constraints related to vehicle capacity, time windows, and route connectivity. The model is implemented using the Julia JuMP optimization package, which provides a flexible and efficient framework for modeling and solving large-scale mathematical programs.

2. Column Generation Approach:
As an alternative to MILP, this approach reformulates the problem using a potentially exponential set of feasible routes. Starting with a set of trivial routes—each serving a single customer—the method iteratively solves a restricted master problem and a pricing subproblem to identify and add new routes that improve the solution. This decomposition-based method significantly enhances scalability, especially for larger problem instances.

The dataset used in this project includes customer coordinates and demand values, with the depot specified as the final entry. Travel times are computed using Euclidean distance, ensuring realistic routing costs. The implementation notebook includes both optimization strategies, performance comparisons, and visualizations of the resulting vehicle routes.

This project showcases expertise in combinatorial optimization, integer programming, and decomposition techniques, and demonstrates practical skills in leveraging Julia for solving real-world logistics and transportation problems. It offers a robust foundation for applications in supply chain optimization and intelligent transportation systems.
