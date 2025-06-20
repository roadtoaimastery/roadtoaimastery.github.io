---
layout: post
title: learning_linear_algebra_study_guide
date: 2025-06-19 12:14 -0700
---

# Linear Algebra Summary and Applications (Tutor-Style)

## What’s Linear Algebra? (Professor Summary)

Linear algebra is the branch of mathematics concerned with vector spaces, linear transformations, and systems of linear equations. At its core, it studies how vectors and matrices can represent and manipulate data, often revealing structure through operations like dot products, eigenvalues, and matrix factorizations.

### Applications:
1. **Computer Graphics**  
   - Creates and manipulates 3D scenes using matrices and vectors.  
   - Matrices handle rotation, scaling, and translation.  
   - Vectors represent positions and directions in space.

2. **Machine Learning**  
   - Models learn from data organized in matrices.  
   - Involves operations like gradient descent and linear mappings.  
   - Uses concepts like dot product, SVD, and eigendecomposition.

3. **Quantum Mechanics**  
   - Describes physical systems using vector spaces (Hilbert spaces).  
   - Measurements are eigenvalues; quantum states are eigenvectors.  
   - Operators are linear transformations on these spaces.

---

## 1-Page Cheat Sheet for Linear Algebra

### 🧠 Linear Algebra Cheat Sheet  
_Core Concepts + Applications in Graphics, ML, Quantum Physics_

---

### 📌 Vectors & Vector Spaces
- **Dot Product**:  
  \[
  \mathbf{a} \cdot \mathbf{b} = \sum a_i b_i = \|\mathbf{a}\|\|\mathbf{b}\|\cos\theta
  \]

- **Cross Product** (3D only):  
  \[
  \mathbf{a} \times \mathbf{b} = \text{gives perpendicular vector}
  \]

---

### 📌 Matrices & Linear Maps
- **Matrix multiplication**:  
  \[
  C = AB, \quad C_{ij} = \sum_k A_{ik} B_{kj}
  \]

- **2D Transformations**: rotation, scaling, translation (homogeneous coords)

---

### 📌 Solving \( A\vec{x} = \vec{b} \)
- **Inverse**:  
  \[
  \vec{x} = A^{-1} \vec{b}
  \]

- **Pseudoinverse** (for ML):  
  \[
  A^+ = (A^T A)^{-1} A^T
  \]

---

### 📌 Matrix Properties
- **Determinant**: \( \det(A) \neq 0 \) ⇒ invertible  
- **Trace**: \( \text{tr}(A) = \sum A_{ii} \)  
- **Rank**: number of linearly independent rows/columns

---

### 📌 Eigenvalues & Eigenvectors
- Equation:  
  \[
  A\vec{v} = \lambda \vec{v}
  \]
- Found by solving \( \det(A - \lambda I) = 0 \)

---

### 📌 Orthonormality
- **Projection**:  
  \[
  \text{proj}_{\vec{a}} \vec{b} = \frac{\vec{a} \cdot \vec{b}}{\|\vec{a}\|^2} \vec{a}
  \]

---

### 📌 Singular Value Decomposition (SVD)
- Decomposition:  
  \[
  A = U \Sigma V^T
  \]
- Used in compression, ML, quantum state structure

---

### 🔚 Applications Table

| Concept       | Graphics     | Machine Learning       | Quantum Mechanics         |
|---------------|--------------|-------------------------|----------------------------|
| Transforms    | Matrices     | Feature spaces          | State evolution           |
| Dot Product   | Lighting     | Similarity, kernels     | Inner product of states   |
| Eigenvalues   | NA           | PCA, optimization       | Observable measurement    |
| SVD           | NA           | Data compression        | Quantum state structure   |

---

## Application Breakdown – Tutor for a 10-Year-Old

---

### Application 1: Transforms (Graphics)

**Goal**: Move, spin, and scale objects using **vectors and matrices**.

Steps:
1. Vectors = positions (e.g., where a LEGO figure is).
2. Matrices = how to rotate, scale, or move objects.
3. Multiply Matrix × Vector to get a new position.
4. Use special matrices for each action (rotate, scale, translate).
5. Combine multiple actions by multiplying matrices.
6. Games use this every frame to update object positions on screen.

---

### Application 2: Dot Product (Lighting in Graphics)

**Goal**: Figure out **how bright** something looks when a light hits it.

Steps:
1. Represent light direction and surface direction as vectors.
2. Use the dot product to find how aligned they are.
3. Dot product formula:  
   \[
   \vec{a} \cdot \vec{b} = \|\vec{a}\|\|\vec{b}\|\cos\theta
   \]
4. Big dot product = bright light; small = dim; negative = no light.
5. Used in every lighting and shading system in games.

---

### Application 3: Eigenvalues (Quantum Physics)

**Goal**: Find directions that don’t rotate under transformation — they just stretch/shrink.

Steps:
1. A matrix transforms vectors (stretches/rotates them).
2. Eigenvectors are special vectors that don’t rotate — just scale.
3. Equation:  
   \[
   A\vec{v} = \lambda \vec{v}
   \]
4. λ = eigenvalue (how much it stretches/shrinks).
5. In quantum mechanics: eigenvalues = measurement outcomes, eigenvectors = possible states.

---

### Application 4: SVD (Data Compression & ML)

**Goal**: Break a big messy matrix into neat parts.

Steps:
1. Matrix = data (like a photo or table).
2. SVD splits it into 3 parts:  
   \[
   A = U \Sigma V^T
   \]
   - U = direction info  
   - Σ = importance (singular values)  
   - Vᵗ = how things are arranged
3. Keep only the big values in Σ to compress or simplify the data.
4. Used in ML for pattern recognition, compression, and reducing noise.

---

