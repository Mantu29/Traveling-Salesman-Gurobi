# Traveling Salesman Problem Solver with Gurobi

## Overview

This repository contains a Jupyter Notebook that implements solutions to the Traveling Salesman Problem (TSP) using the Gurobi Optimizer. The notebook explores two approaches to solve the TSP, ensuring a comprehensive understanding of its solutions.

## Input File Format

The TSP instances are provided in a text file named `TSP_instance.txt`. The file format is a square matrix where each row represents a city, and each column within that row represents the distance to every other city. Distances are separated by spaces or commas, and each row is on a new line.

## Solution Approaches

The notebook implements two distinct approaches to solve the TSP:

1. **Direct Solution**: This approach directly uses Gurobi's optimization capabilities to find the optimal TSP route by defining the necessary decision variables, constraints (including subtour elimination constraints), and the objective function to minimize the total distance.

2. **Iterative Subtour Elimination**: In this approach, the model initially ignores the subtour elimination constraints and solves the TSP. It then checks the solution for subtours and iteratively adds subtour elimination constraints until the solution contains no subtours, ensuring a valid TSP tour.

## Getting Started

### Prerequisites

- Python 3.x
- Jupyter Notebook or JupyterLab
- Gurobi Optimizer (with a valid license)

### Gurobi Setup

Follow the [Gurobi Documentation](https://www.gurobi.com/documentation/) for installation instructions and license setup.

### Installation

1. Clone the repository and navigate to it:

    ```bash
    git clone https://github.com/your_username/TSP_Solver_Gurobi.git
    cd TSP_Solver_Gurobi
    ```

2. (Optional) Set up a virtual environment and activate it.

3. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Running the Notebook

Launch Jupyter and open the `TSP_Solver_Gurobi.ipynb` notebook. Follow the instructions within the notebook to run the TSP solver.

## Contributing

Contributions are welcome. Please fork the repository, make your changes, and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
