# Multimodal Function Optimization using Genetic Algorithms

An evolutionary computation project focusing on complex function optimization, diversity maintenance, and restricted mating.

## 📌 Project Overview

The objective is to find the global maximum of a continuous, highly multimodal 2D mathematical function. Due to the presence of numerous local optima, standard Genetic Algorithms typically suffer from premature convergence (the entire population getting stuck on a suboptimal peak). 

This project implements and evaluates strategies to maintain population diversity and successfully locate the true global maximum.

### Key Highlights:
- **Standard Genetic Algorithm:** Implemented with real-valued encoding, Tournament Selection, Simulated Binary Crossover (SBX), and Polynomial Mutation.
- **Fitness Sharing:** Reduces the fitness of individuals that are clustered closely together, promoting the exploration of multiple peaks simultaneously (niche formation).
- **Restricted Mating (Speciation):** Restricts crossover to individuals that are within a certain distance of each other to prevent the creation of "lethal" offspring that fall into the valleys between peaks.

## 🛠️ Technologies Used
- **Python 3**
- **NumPy**
- **Matplotlib** (3D surface plots and 2D contour mapping)

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/Aleksander-Romanha/multimodal-genetic-algorithm-optimization.git
   cd multimodal-ga-optimization
   ```

2. Open the Jupyter Notebook:
   ```bash
   jupyter notebook multimodal_genetic_algorithm_optimization.ipynb
   ```

## 📈 Results
- **Standard GA**: Tends to prematurely converge all individuals onto a single local peak.
- **Fitness Sharing**: Successfully maintains diverse sub-populations across multiple peaks, enabling broader exploration.
- **Restricted Mating**: Enhances speciation by preventing crossover between distinct species, resulting in tighter clusters around the optimal peaks and a higher success rate in finding the global optimum.
