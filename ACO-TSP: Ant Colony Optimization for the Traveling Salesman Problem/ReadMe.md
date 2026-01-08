# ACO-TSP: Ant Colony Optimization for the Traveling Salesman Problem

This project implements the **Ant Colony Optimization (ACO)** algorithm to solve the **Traveling Salesman Problem (TSP)** for small-scale instances. ACO is a bio-inspired metaheuristic where artificial ants iteratively construct tours based on pheromone levels and inverse distances between cities.

## 🎯 Objective

The goal is to find the shortest possible route that visits each city exactly once and returns to the starting point, using ACO to simulate natural ant behavior in finding optimal paths.

## 🧠 Key Features

- **Bio-inspired algorithm**: Simulates ant foraging behavior using pheromone trails.
- **Probabilistic decision-making**: Ants choose next cities based on pheromone intensity and distance.
- **Pheromone update mechanism**: Pheromone levels are updated after each iteration to reinforce good paths.
- **Reproducible results**: The implementation reliably finds optimal or near-optimal solutions for small TSP instances.

## 🛠️ Implementation Details

- **Algorithm**: Ant Colony Optimization (ACO)
- **Problem**: Traveling Salesman Problem (TSP)
- **Parameters**:
  - Pheromone evaporation rate
  - Pheromone influence weight
  - Heuristic (distance) influence weight
  - Number of ants
  - Number of iterations
- **Input**: Distance matrix or set of 2D coordinates
- **Output**: Optimal or near-optimal tour and total path length

## 📊 Experimental Results

The ACO implementation successfully finds optimal or near-optimal TSP tours for small instances. Visualizations (e.g., plots of best tour, convergence over iterations) are included to support the results.

## 🧪 How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/aco-tsp.git
