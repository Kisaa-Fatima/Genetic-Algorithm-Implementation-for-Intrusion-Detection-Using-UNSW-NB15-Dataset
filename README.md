# Genetic-Algorithm-Implementation-for-Intrusion-Detection-Using-UNSW-NB15-Dataset
This project implements a Genetic Algorithm (GA) for the classification of intrusions using the UNSW-NB15 network intrusion dataset. The dataset contains nine different attack types, including DoS, worms, backdoors, and fuzzers. The training set comprises 175,341 records, and the testing set includes 82,332 records of both attack and normal types.

**Overview**
The motivation behind this project is to explore the effectiveness of genetic algorithms in classifying network intrusions. By leveraging the UNSW-NB15 dataset and implementing GA, we aim to enhance intrusion detection systems.

**Base Paper**
The implementation details of the Genetic Algorithm are inspired by the paper:

"An Evolutionary Approach to Intrusion Detection System using Genetic Algorithm"

**Dataset**
-Source: UNSW-NB15 Dataset
-Records: 175,341 (training), 82,332 (testing)
-Attacks: Nine types including DoS, worms, backdoors, and fuzzers.
**Requirements**
-Experiments: Conduct at least three experiments by varying parameters like population size, crossover type, and mutation rate.
-Code: Provide a zip folder containing all the code files with a clear and simple Python run file to initiate the code.
-Report: Prepare a report with evaluation results in a tabular format, explaining the choices made during the implementation.
**Fitness Function**
The fitness function used in this implementation is simple and straightforward, calculating the total sum of all selected features in the dataset. Here’s why this fitness function was chosen:
-Simplicity: Easy to implement and computationally efficient.
-Feature Importance: Implicitly considers the importance of each feature.
-Scalability: Can handle datasets with varying numbers of features without modification.
**Optimization Strategies**
-Early Stopping: Stop early based on conditions like fitness threshold or lack of improvement.
-Optimize Fitness Function: Optimize or find alternative approaches to calculate the fitness function efficiently.
-Reduce Population Size: Balance between runtime and solution quality.
-Reduce Number of Generations: Find an optimal number of generations for acceptable results within reasonable runtime.
-Parallelization: Use libraries such as multiprocessing, threading, and Dask.
**Results**
-Crossover Type: One-point and two-point crossover yield similar fitness values.
-Mutation Rate: Moderate mutation rates (e.g., 0.01 or 0.05) perform better than high mutation rates (0.1).
**Training and Testing Fitness**
-Training Fitness: Shows the algorithm's performance on the training data.
-Testing Fitness: Indicates the algorithm’s generalization ability on unseen data.
**Optimal Configuration**
-Population Size: 100
-Crossover Type: One-point crossover
-Mutation Rate: 0.01
This configuration achieves relatively high fitness values on both the training and testing datasets, indicating good generalization ability.

**Experiments**
Three experiments were conducted with varying parameters to evaluate the GA’s performance:

-Population Sizes: 50, 100, 200
-Crossover Types: One-point, two-point
-Mutation Rates: 0.01, 0.05, 0.1
**Evaluation**
The selected parameters provide a structured approach to evaluating the genetic algorithm's performance while keeping the experimentation process manageable. The results highlight how changes in these parameters affect the GA's performance.
