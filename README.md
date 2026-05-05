# Modernizing the AMPL Stack

This repository contains supporting materials for a two-part webinar series on modernizing the AMPL workflow. It is designed for academics, researchers, and students who want to transition from legacy AMPL usage to a modern, Python-based integration.

## Overview

The webinar is divided into two logical phases:

1.  **Part One: Conceptual Evolution**
    *   Discussion on the evolution of the AMPL ecosystem.
    *   Identifying what remains foundational and what has been modernized.
    *   Located in the [`part-one/`](./part-one/) directory.

2.  **Part Two: Hands-on Migration**
    *   A practical guide to migrating from standalone `.mod`, `.dat`, and `.run` files to a Pythonic workflow using `amplpy`.
    *   Demonstration of data management with Pandas and visualization with Matplotlib.
    *   Located in the [`part-two/`](./part-two/) directory.

## Repository Structure

```text
modern-ampl/
├── part-one/
│   └── ampl_part1.pdf          # Presentation slides/document for Part 1
└── part-two/
    ├── diet.mod                # AMPL Model file (Diet Problem)
    ├── diet.dat                # Legacy AMPL Data file
    ├── diet.run                # Legacy AMPL Run file
    └── webinar_part_two.ipynb  # Main Hands-on Jupyter Notebook
```

## Key Features & Topics Covered

### 1. Modern Python Integration
Move away from the rigid standalone IDE and leverage the full power of the Python ecosystem. The `amplpy` library allows you to:
*   Load AMPL models directly into Python.
*   Use **Pandas DataFrames** instead of `.dat` files for dynamic and robust data handling.
*   Solve models using various solvers (HiGHS, Gurobi, CPLEX, etc.) with simple Python commands.

### 2. Visualization and Results Analysis
*   Extract results directly into Pandas structures for post-processing.
*   Create professional plots and dashboards using **Matplotlib** and **Streamlit**.
*   Perform "What-If" analysis by updating parameters dynamically in Python.

### 3. Advanced Diagnostic Tools
*   **IIS (Irreducible Infeasible Subset):** Learn how to diagnose infeasible models using modern solver features.
*   **Dual Values & Sensitivity:** Access dual values for economic interpretation and sensitivity analysis.
*   **Snapshots:** Save and restore complete AMPL sessions for warm-starts or grading purposes.
*   **ampls:** Explore lightweight interfaces for advanced solver interactions and custom callbacks.

## Getting Started

To follow the hands-on session:

1.  Navigate to the `part-two/` directory.
2.  Open `webinar_part_two.ipynb` in a Jupyter environment (JupyterLab, VS Code, or Google Colab).
3.  Install the necessary requirements (included in the notebook):
    ```bash
    pip install amplpy pandas matplotlib
    ```
4.  Follow the step-by-step instructions in the notebook to migrate the "Diet Problem" to a modern stack.

## Additional Resources

*   **AMPL Model Colaboratory:** [colab.ampl.com](https://colab.ampl.com/) - A library of ready-to-run notebooks.
*   **AMPL Python API Docs:** [amplpy.ampl.com](https://amplpy.ampl.com/)
*   **AMPL Resources:** [ampl.com/resources](https://ampl.com/resources/)
*   **AMPL Streamlit Apps:** [amplopt.streamlit.app](https://amplopt.streamlit.app/)

---
*Created for the "Moving Your Course to Modern AMPL" Webinar series.*
