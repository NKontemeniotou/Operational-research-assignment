# 🏗️ Residential Development Optimization Report

This report presents the solution to a real estate investment problem involving the optimal allocation of land and capital for the construction of two types of residential units: **maisonettes** and **apartments**.

---

## 📌 Project Overview

A developer has acquired a **plot of land measuring 80,000 m²** and intends to build a combination of two housing types:

- **Maisonettes**
- **Apartments**

The developer has an available capital of **€40,000,000**, but can receive advance payments depending on unit type:
- **30% advance** from the sale of each **maisonette**
- **25% advance** from the sale of each **apartment**

---

## 📊 Construction Data

| Property Type | Maisonette | Apartment |
|---------------|------------|-----------|
| **Quantity**  | x          | y         |
| **Area per unit** | 400 m² | 240 m² |
| **Construction cost per unit** | €420,000 | €250,000 |
| **Profit per unit** | €350,000 | €170,000 |
| **Selling price** | €770,000 | €420,000 |

---

## ⚖️ Constraints

1. **Land Usage**: Maximum **60% of the land (48,000 m²)** may be used for construction.  
   - If exceeded, **30% chance** of fine: €1,000 per m² of excess area.

2. **Total Units Limit**:  
   - Maximum **150 total residential units** (x + y ≤ 150)

3. **Minimum Units Condition**:  
   - Either **at least 15 maisonettes and 15 apartments**, or **none at all** of a type.

4. **Balance Condition** (if both types built):  
   - The number of **apartments must be at least double** the number of maisonettes → y ≥ 2x

---

## 🎯 Objective

**Maximize total profit**, considering:
- Construction costs
- Selling profits
- Potential advance payments
- Constraint compliance
- Risk of penalty for excess land usage

---

## 🧮 Decision Variables

- `x`: Number of maisonettes
- `y`: Number of apartments

---

## 💡 Suggested Use

This formulation is ideal for solving via **Linear Programming** technique in tools such as:
- Excel Solver

