# University of Puerto Rico at Mayagüez  
### Department of Electrical and Computer Engineering   
#### ICOM5015 - Artificial Intelligence  

**Project Title:** Python Performance with and without NumPy  
**Assignment:** Programming Assignment 1 – Performance Benchmarking  
**Team:** Group M  
- **Marco Yu** – Undergraduate, Computer Science  
- **Samir Rivera** – Undergraduate, Software Engineering  

**Professor:** J. Fernando Vega Riveros   
**Date:** Febrruary 21, 2025  

<p align="center">
  <img src="https://www.uprm.edu/wdt/resources/seal-rum-uprm-1280x1280px.png" alt="UPRM Logo" width="250" height="250">
</p>

---

# Python Performance with and without NumPy  
**Performance Benchmarking of Array Operations in Pure Python and NumPy**  

---

## 🧠 **Project Overview**

This assignment investigates the computational efficiency of **pure Python** versus **NumPy** when performing element-wise array multiplications across increasing data sizes. The goal is to highlight the importance of optimized libraries like NumPy in scientific computing.

Key concepts:
- Vector and matrix operations
- Algorithmic complexity and performance scaling
- Optimization through compiled extensions (C underpinnings of NumPy)

---

## 🔬 **Assignment Objectives**

- Implement element-wise array multiplication using **pure Python loops** and **NumPy operations**
- Compare execution times for varying array sizes (1D and 2D)
- Analyze and explain performance differences
- Present results through **graphs** and **tables**
- Reflect on the role of NumPy in Python’s numerical computing ecosystem

---

## 🧪 **Experiment Design**

### Array Sizes Tested:
- **1D Arrays:** 10, 50, 100, 200, 500 elements  
- **2D Matrices:** 10×10, 50×50, 100×100, 200×200, 500×500  

Each configuration was tested using both implementations with average runtime calculated over 10 iterations.

### Multiplication Methods:
| Method        | Description                        |
|---------------|------------------------------------|
| Pure Python   | Iterative element-wise multiplication using lists |
| NumPy         | Vectorized operations leveraging internal optimizations |

---

## 📁 **Repository Contents**

| File | Description |
|------|-------------|
| `Group_M_programming_assignment_1.ipynb` | Jupyter notebook with source code, analysis, and visualizations |
| `benchmark_results.csv` | Raw data of benchmark results |
| `benchmark_results_table.png` | Table summary of execution times |
| `1d_performance.png` | Line plot: performance vs size for 1D arrays |
| `2d_performance.png` | Line plot: performance vs size for 2D matrices |
| `Programming Assignment 1.docx` | Final report (non-text) |
| `Python_vs_NumPy_Presentation.pptx` | Presentation slides (non-text) |

---

## 📈 **Results and Analysis**

### Performance Summary:
NumPy significantly outperforms pure Python, especially for large arrays. The time complexity of Python’s interpreted loops scales poorly compared to NumPy's compiled, vectorized operations.

| Tipo | Tamaño | Tiempo_Python (s) | Tiempo_NumPy (s) |
|------|--------|-------------------|------------------|
| 1D   | 10     | 1.69e-06          | 2.29e-06         |
| 1D   | 500    | 3.63e-05          | 1.62e-06         |
| 2D   | 50×50  | 5.82e-04          | 2.85e-04         |
| 2D   | 500×500| 0.0301            | 0.0005           |

See visualizations in:
- `1d_performance.png`
- `2d_performance.png`

---

## 🧵 **Code Structure**

The project is fully implemented in a single, well-organized Jupyter Notebook:
- Functions for 1D and 2D multiplication (Python and NumPy)
- Benchmarking function with repeated trials
- CSV export of results
- Data visualization using `matplotlib` and `pandas`

---

## 👥 **Team Collaboration**

- **Marco Yu** – Implemented NumPy benchmarks and plots; contributed to analysis  
- **Samir Rivera** – Implemented pure Python methods and data recording; handled report writing  

All members participated in video production and presentation.

---

## 🎥 **Presentation Video**

A 5-minute summary of our methodology, code, and findings is available at:  
🔗 [Video Link](https://www.youtube.com/watch?v=xuzfuV-kYNM&t=1s)

---

## 📚 **References**

- NumPy Documentation: https://numpy.org/doc/
- Python Official Docs: https://docs.python.org/3/
- IEEE Format Citations included in the final report

---

## 📌 **Conclusion**

Through this assignment, we observed that:
- Pure Python is readable and easy to use but lacks speed at scale.
- NumPy, written in C, leverages optimized memory access and parallelism.
- Performance testing and visualization are key to understanding algorithmic trade-offs.

This experiment reinforces the importance of choosing the right tool for data-intensive computing.