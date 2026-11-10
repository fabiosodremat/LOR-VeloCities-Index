<div align="center">

# L’OR VeloCities Index

### A Mathematical Model of Urban Rhythm

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy">
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas">
  <img src="https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white" alt="Matplotlib">
</p>

<a href="https://colab.research.google.com/github/fabiosodremat/LOR-VeloCities-Index/blob/main/lor_velocities_index.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Google Colab">
</a>

<br>

*Understanding the rhythm of cities through mathematics.*

</div>

---

## Overview

**How fast does a city live?**

The L’OR VeloCities Index is a mathematical modeling project developed to quantify and compare the rhythm of urban environments.

The model combines two fundamental dimensions of urban life:

- **Population density:** the spatial concentration of people.
- **Commuting time:** the temporal cost of urban mobility.

By combining these variables through nonlinear transformations and normalization, the project constructs a dimensionless index representing relative urban intensity.

The conceptual framework draws inspiration from Robert V. Levine's research on cultural differences in the perception and organization of time.

## The Mathematical Model

Let \(D_i\) denote population density and \(T_i\) the average one-way commuting time for city \(i\).

### 1. Urban Load Index

The model begins by defining:

$$
URI_i = D_i \cdot T_i
$$

This functional combines spatial density and temporal expenditure into a measure of urban intensity.

### 2. Nonlinear Transformation

A square root transformation is applied:

$$
X_i = \sqrt{URI_i}
$$

This transformation compresses the scale of the original observations.

### 3. Geometric Normalization

The geometric mean of the transformed observations is:

$$
\bar{X}_g =
\exp\left(
\frac{1}{n}
\sum_{i=1}^{n}\ln X_i
\right)
$$

The normalized index is then defined as:

$$
R_i^{(base)} = \frac{X_i}{\bar{X}_g}
$$

### 4. Final Rescaling

Finally, the normalized values are rescaled so that the maximum observation equals 2.0:

$$
R_i =
2 \cdot
\frac{R_i^{(base)}}{R_{\max}}
$$

where:

$$
R_{\max} = \max_i R_i^{(base)}
$$

The resulting index satisfies:

$$
0 < R_i \leq 2
$$

The final scale is analogous to media playback speed, providing an accessible way to communicate differences in urban intensity.

> **Mathematical note:** The geometric mean appears explicitly in the original normalization procedure. Since it is common to all observations, it cancels algebraically in the final rescaling. The implementation preserves the original computational sequence.

## Results

The model was applied to 14 selected locations.

| City | VeloCities Index |
|:--|--:|
| Mexico City | **2.00x** |
| New York City | 1.95x |
| São Paulo | 1.66x |
| Rio de Janeiro | 1.42x |
| Shanghai | 1.39x |
| London | 1.37x |
| Brussels | 1.36x |
| Tokyo | 1.35x |
| Paris | 1.29x |
| Berlin | 1.00x |
| Amsterdam | 0.99x |
| Oslo | 0.54x |
| Capri | 0.35x |
| Santorini | 0.16x |

The results are relative to the selected sample. Mexico City establishes the upper reference value of 2.0x.

## Computational Implementation

The complete model was implemented in Python using:

| Technology | Purpose |
|:--|:--|
| Python | Computational implementation |
| NumPy | Numerical operations and mathematical transformations |
| Pandas | Dataset organization and manipulation |
| Matplotlib | Data visualization |

The Jupyter Notebook includes:

- Dataset construction.
- Urban Load Index calculation.
- Nonlinear transformation.
- Geometric mean normalization.
- Final index computation.
- Ranking table.
- Scatter plot of the relationship between URI and the final index.

## Conceptual Background

The theoretical inspiration comes from:

**Levine, R. V. (1997).** *A Geography of Time: The Temporal Misadventures of a Social Psychologist.*

The research explores how cultural and geographical contexts influence the perception and organization of time.

The VeloCities project connects these ideas with observable urban characteristics, translating demographic and mobility data into a quantitative representation of urban rhythm.

## Contributions

**Adriana Alves**
- Strategic conception and research direction.
- Theoretical and journalistic research.
- Data collection and curation.
- Conceptual framework and communication strategy.

**Fábio Sodré Rocha, PhD in Mathematics**
- Mathematical formulation and development of the quantitative model.
- Definition of mathematical transformations and normalization procedures.
- Computational implementation in Python.
- Numerical analysis and visualization.

The project combines strategic research, data curation, mathematical modeling and computational development.

## Repository Structure

```text
LOR-VeloCities-Index/
│
├── README.md
│
└── lor_velocities_index.ipynb
```

## Methodological Considerations

The index is a constructed comparative metric based on population density and average one-way commuting time.

Its interpretation depends on the consistency and comparability of the underlying data, including geographical boundaries, population definitions and commuting-time sources.

The results should be interpreted as comparisons within the selected dataset, rather than as universal or empirically validated measurements of urban rhythm.

---

<div align="center">

**L’OR VeloCities Index**

*Mathematics, data and the rhythm of urban life.*

</div>
