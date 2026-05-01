# MLB Optimization Model

## Overview
This project builds an optimization model to select the highest scoring DraftKings MLB lineup using real game data.

## Objective
Maximize total DraftKings fantasy points while staying under salary and roster constraints.

## Tools Used
- Python (Pyomo)
- Pandas
- Integer Programming

## Data
- MLB game data pulled via API  
- DraftKings player and salary data  

## Methodology
- Calculated DraftKings scoring from real player statistics  
- Built an optimization model with salary and roster constraints  
- Solved using integer programming to generate the optimal lineup  

## Results

### Optimization Model (Actual Results Benchmark)
**Total Salary Used:** $49,300  
**Total Actual Points:** 268.15  

The model generated a high-performing lineup while satisfying all constraints.

---

### Strategy Comparison: Weak Opponent Model
**Total Salary Used:** $49,900  
**Projected Points:** 128.32  
**Actual Points:** 79.00  

This strategy prioritizes players facing weaker opponents but significantly underperformed compared to the optimization model.

---

### Simple Average-Based Strategy (Naive Baseline)
**Total Salary Used:** $49,900  
**Total Avg Points Per Game:** 124.96  
**Total Actual Points:** 62.00  

This approach selects players based only on average points per game, without using optimization or matchup adjustments.

---

## Key Insight
The optimization model (268.15 points) significantly outperformed both alternative approaches:

- Weak opponent strategy: 79.00 points  
- Naive average-based strategy: 62.00 points  

This demonstrates that simple selection strategies are not effective under multiple constraints, and that optimization provides a much stronger approach by evaluating all variables simultaneously.

---

## Project Structure
- notebooks/: main model and analysis  


## How to Run
File paths may need to be updated depending on your local setup or environment.
