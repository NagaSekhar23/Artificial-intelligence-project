Evolutionary N-Queens Solver
# Evolutionary N-Queens Solver

A Python implementation of an Evolutionary Algorithm (EA) to solve the classic 8-Queens problem — placing 8 queens on a chessboard such that no two queens threaten each other.

## Problem Statement

The goal is to find a non-attacking arrangement of 8 queens on an 8×8 chessboard. No two queens should share the same row, column, or diagonal.

## Methodology

This project uses an **Evolutionary Algorithm** to search for optimal solutions. Key components include:

- **Solution Representation**: Each individual is a permutation of `[1..8]`, where the value at index `i` represents the row of the queen in column `i`. This ensures no row or column conflicts.
- **Fitness Function**: Measures the number of non-attacking pairs (maximum = 28), penalizing diagonal threats.
- **Crossover**: Ordered Crossover (OX) preserves the permutation structure.
- **Mutation**: Swap Mutation randomly swaps two elements in the permutation.
- **Selection**: Tournament Selection ensures selection pressure while maintaining diversity.
- **Hyperparameters**: Tuned for a balance between exploration and convergence.

## Results

The EA demonstrates robust performance in finding valid solutions. The permutation-based encoding, combined with OX crossover and swap mutation, enables efficient convergence to optimal or near-optimal configurations.

## Features

- Implementation of EA with customizable parameters.
- Fitness evaluation for diagonal and non-attacking constraints.
- Visualization of solutions (optional).
- Configurable tournament size and mutation rate.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/evolutionary-nqueens.git
