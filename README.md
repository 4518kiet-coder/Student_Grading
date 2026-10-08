🎓 Student Grade Curving System (A8)

📌 Project Overview

The Student Grade Curving System is a B.Tech Mathematics mini project that normalizes student grades when the same subject is taught by three professors with different examination difficulty levels.

The system compares the mean and standard deviation of the three groups and applies an affine transformation to place them on a common statistical scale.

---

🎯 Problem Statement

Three professors teaching the same subject may conduct examinations with different difficulty levels.

Therefore, the three groups may have different:

- Mean
- Variance
- Standard deviation
- Grade distributions

The objective is to scale the grades so that the groups have a common statistical scale.

---

🧮 Mathematical Model

The project uses the affine transformation:

[
y = ax + b
]

where:

- "x" = Original grade
- "y" = Adjusted grade
- "a" = Scaling factor
- "b" = Shift factor

The scaling factor is:

[
a = \frac{\text{Target SD}}{\text{Original SD}}
]

The shift factor is:

[
b = \text{Target Mean} - a(\text{Original Mean})
]

This transformation makes the adjusted grades have the selected target mean and standard deviation.

Mathematical Assumption

We do not invent an arbitrary 3×3 formula.

Mean and standard-deviation matching alone does not uniquely define an arbitrary 3×3 linear system. Therefore, the project uses the standard affine normalization model "y = ax + b".

A separate 3×3 Gaussian elimination solver is implemented to demonstrate the required linear algebra concept.

---

🔢 Gaussian Elimination

The project implements Gaussian elimination for solving a 3×3 system:

[
AX = B
]

Example:

2x + y - z   = 8
-3x - y + 2z = -11
-2x + y + 2z = -3

Solution:

x = 2
y = 3
z = -1

The solution is also verified using matrix multiplication.

---

🌍 Real-World Context

Grade normalization can be useful when:

- Different professors teach the same subject.
- Different sections have different examination difficulty.
- Different batches have different grade distributions.
- Student performance needs to be compared on a common scale.

---

✨ Features

- Dynamic grade input
- Mean calculation
- Variance calculation
- Standard deviation calculation
- Grade normalization
- Scaling factor calculation
- Shift factor calculation
- 3×3 Gaussian elimination
- Numerical verification
- Before/after comparison
- Statistical charts
- Interactive Gradio front end

---

💻 Technologies Used

- Python
- NumPy
- SymPy
- Matplotlib
- Gradio
- Google Colab

---

📊 Sample Dataset

Professor 1

45 50 55 60 65

Professor 2

55 60 65 70 75

Professor 3

35 45 55 65 75

---

📈 Visualizations

The project generates charts for:

1. Original vs adjusted mean
2. Original vs adjusted standard deviation
3. Original vs adjusted grade distributions

---

🚀 How to Run

Google Colab

1. Open the project notebook in Google Colab.
2. Install the required libraries.
3. Run the import cell.
4. Enter grades for the three professors.
5. Run the mathematical model.
6. Run the grade normalization.
7. View the results and charts.
8. Launch the Gradio front end.

---

📦 Required Libraries

numpy
sympy
matplotlib
gradio

Install using:

pip install numpy sympy matplotlib gradio

---

🏗️ Project Workflow

User Input
    ↓
Calculate Mean & Standard Deviation
    ↓
Select Target Mean & Standard Deviation
    ↓
Construct Mathematical Model
    ↓
Calculate Scaling Factor (a)
    ↓
Calculate Shift Factor (b)
    ↓
Adjust Grades
    ↓
Verify Mean & Standard Deviation
    ↓
Display Results
    ↓
Generate Charts

---

📁 Project Structure

Student-Grade-Curving-System/
│
├── README.md
├── grade_curving.ipynb
├── app.py
├── requirements.txt
│
└── images/
    ├── mean_comparison.png
    ├── standard_deviation.png
    └── grade_distribution.png

---

🎓 Learning Outcomes

This project demonstrates the practical application of:

- Linear algebra
- Matrices
- Gaussian elimination
- Mean
- Variance
- Standard deviation
- Statistical normalization
- Python programming
- Data visualization

---

🔮 Future Enhancements

- CSV/Excel grade upload
- Student names and IDs
- Automatic letter-grade generation
- GPA calculation
- Multiple-section support
- Downloadable reports
- Interactive dashboard
- Web deployment

---

👨‍💻 Project Information

Project: Student Grade Curving System (A8)
Type: B.Tech Mathematics Mini Project
Core Concepts: Linear Algebra + Statistics + Python
