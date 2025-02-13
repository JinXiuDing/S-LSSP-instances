# Dataset Introduction

## 1. Source and Modification of Computational Instances
In our study, we employed computational instances based on those developed by Ruiz and St ̈utzle, which are designed for the basic flowshop scheduling problem. To align these instances with the specific requisites of our research, modifications are made to the due dates and the setup times between identical jobs.

## 2. Generation of Processing Times
The processing times were generated from a uniform distribution in the range of [1,99].

## 3. Classification of Instances Based on Setup - Time to Processing - Time Ratio
The instances were classified into four categories based on the ratio of set - up time to processing time, namely SDST10, SDST50, SDST100, and SDST125.
- **Major Setup Times**:
    - For SDST10, major setup times were randomly generated from a uniform distribution spanning [1,9].
    - For SDST50, major setup times were randomly generated from a uniform distribution spanning [1,49].
    - For SDST100, major setup times were randomly generated from a uniform distribution spanning [1,99].
    - For SDST125, major setup times were randomly generated from a uniform distribution spanning [1,124].
- **Minor Setup Times**:
    - For SDST10, minor setup times were randomly generated from a uniform distribution spanning [1,5].
    - For SDST50, minor setup times were randomly generated from a uniform distribution spanning [1,25].
    - For SDST100, minor setup times were randomly generated from a uniform distribution spanning [1,50].
    - For SDST125, minor setup times were randomly generated from a uniform distribution spanning [1,75].

## 4. Due Date Distributions
In terms of due dates, the instances are characterized by diverse distribution types, each denoted by a specific letter:
- U for a uniform distribution.
- E for an exponential distribution.
- N for a normal distribution.

## 5. Datasets Organization
Our instances can be organized into six datasets:

### Dataset 1
- **Number of Instances**: 15 instances.
- **Due Date Distribution**: 5 instances for each due date distribution.
- **Configuration**: Each instance consists of 7 jobs and 5 machines, and the production lot of each job can be divided into no more than 3 sublots (denoted as 7 - 3 - 5).
- **Purpose**: Utilized for exploring the value of stochastic information.

### Dataset 2
- **Number of Instances**: 60 instances.
- **Configuration**: 7 - 3 - 5.
- **Due Date Distribution**: 20 instances in each distribution.
- **Purpose**: Utilized for sensitivity analysis.

### Datasets 3 - 6
- **Number of Instances per Dataset**: 30 instances.
- **Due Date Distribution**: 10 instances for each due date distribution.
- **Configurations**:
    - Dataset 3: 5 - 3 - 5.
    - Dataset 4: 7 - 3 - 5.
    - Dataset 5: 10 - 3 - 5.
    - Dataset 6: 12 - 3 - 8.
- **Purpose**: Employed to validate the efficiency of the proposed algorithms.

## 6. Instance Structure
The instances are structured to sequentially present the processing times, followed by the setup times, and ultimately data related to due date distribution.

### Due Date Distribution Details
- **Normal distribution**: mean, standard deviation.
- **Exponential distribution**: mean.
- **Uniform distribution**: left_bound right_bound.

## 7. Solution Information
- You can view the solution values for each dataset in the `Solution values` folder.
- You can view the solution results in the `numerical result.xlsx` file.
