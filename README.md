# Numerical Lab

A collection of Jupyter notebooks covering fundamental numerical methods and computational techniques in Python.

## Topics Covered

### M1 - Foundations & Error Analysis
- Machine Epsilon calculation (manual and NumPy)
- Binary representation of floating-point numbers (IEEE 754)
- Catastrophic cancellation and numerical stability
- Truncation error in Taylor series approximation
- Summation stability and Kahan's algorithm

### M2 - Algorithms for Data Streams (Online Methods)
- Running average (online mean)
- Mean Absolute Deviation using Welford's algorithm
- Percentile ranking

### M3 - Direct Methods for Linear Systems
- Solving linear systems using NumPy and SciPy
- Random coefficient problems
- Matrix algebra laws verification
- Naive Gaussian elimination (forward elimination)

### M4 - Advanced Linear Algebra and Optimization
- Markov chain convergence (fixed and random)
- Least squares for linear and overdetermined systems
- Linear programming optimization with `scipy.optimize.linprog`

### M5 - Roots of Non-Linear Equations
- Bisection method (vanilla, trisection, and random variants)
- Fixed-point iteration
- Newton's method
- Secant method
- Both manual implementations and SciPy library functions

### M6 - Series Approximation & Interpolation
- Maclaurin series approximation for $\cos(x)$
- Linear interpolation
- Cubic spline interpolation

## Requirements

- Python 3.10+
- NumPy
- SciPy
- Matplotlib
- SymPy
- Pandas
- IPyKernel (for Jupyter notebooks)

## Installation

This project uses [uv](https://docs.astral.sh/uv/) for dependency management.

### Install uv

```bash
# On Windows (PowerShell)
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"

# On macOS/Linux
curl -LsSf https://astral.sh/uv/install.sh | sh
```

### Setup the Project

```bash
# Clone the repository and navigate to the project directory
cd numerical-lab

# Create a virtual environment and install dependencies
uv sync

# Or install dependencies directly
uv pip install -r pyproject.toml
```

### Running Notebooks

```bash
# Activate the virtual environment
# On Windows
.venv\Scripts\activate

# On macOS/Linux
source .venv/bin/activate

# Start Jupyter
jupyter notebook
```

Or open the notebooks directly in VS Code with the Python extension installed.

## Project Structure

```
numerical-lab/
├── M1.ipynb          # Foundations & Error Analysis
├── M2.ipynb          # Online Algorithms for Data Streams
├── M3.ipynb          # Direct Methods for Linear Systems
├── M4.ipynb          # Advanced Linear Algebra & Optimization
├── M5.ipynb          # Roots of Non-Linear Equations
├── M6.ipynb          # Series Approximation & Interpolation
├── main.py           # Entry point script
├── pyproject.toml    # Project configuration and dependencies
├── uv.lock           # Locked dependencies
└── README.md
```

## Usage

Each notebook (`M1.ipynb` through `M6.ipynb`) is self-contained and can be run independently. Simply open the desired notebook and execute the cells sequentially.

## License

This project is for educational purposes.
