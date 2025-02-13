# Flowshop Scheduling Instances Documentation

## Overview
This repository contains computational instances adapted from Ruiz and Stützle's work for the basic flowshop scheduling problem. Modifications have been made to align with our research requirements, specifically:
- **Due dates** adjusted for different distribution types.
- **Setup times** between identical jobs redefined.

---

## Instance Generation

### Processing Times
- Generated from a uniform distribution in the range **[1, 99]**.

### Setup Times
Instances are categorized into four groups based on setup-to-processing time ratios:

| Category  | Major Setup Time Range | Minor Setup Time Range |
|-----------|------------------------|------------------------|
| SDST10    | [1, 9]                 | [1, 5]                 |
| SDST50    | [1, 49]                | [1, 25]                |
| SDST100   | [1, 99]                | [1, 50]                |
| SDST125   | [1, 124]               | [1, 75]                |

### Due Date Distributions
Due dates follow three distribution types:
- **U (Uniform)**: Defined by `[left_bound, right_bound]`
- **E (Exponential)**: Defined by `mean`
- **N (Normal)**: Defined by `mean` and `standard_deviation`

---

## Datasets
Six datasets are provided for different research purposes:

### 1. Dataset 1: Stochastic Information Exploration
- **Size**: 15 instances (5 per distribution)
- **Configuration**: 7 jobs, 3 sublots, 5 machines (`7-3-5`)

### 2. Dataset 2: Sensitivity Analysis
- **Size**: 60 instances (20 per distribution)
- **Configuration**: `7-3-5`

### 3. Validation Datasets (Algorithm Efficiency)
Four datasets with **30 instances each** (10 per distribution):

| Dataset   | Configuration |
|-----------|---------------|
| Dataset 3 | 5-3-5         |
| Dataset 4 | 7-3-5         |
| Dataset 5 | 10-3-5        |
| Dataset 6 | 12-3-8        |

---

## Data Structure
Instance files are organized sequentially as:
1. **Processing Times**
2. **Setup Times**
3. **Due Date Parameters** (specific to distribution type)

---

## Solution Values
- **Solution Values Folder**: Contains optimal/reference values for all instances.
- **Numerical Results**: Full experimental results are provided in `numerical_result.xlsx`.
