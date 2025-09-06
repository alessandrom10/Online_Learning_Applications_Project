# Online Learning for Dynamic Pricing under Production Constraints

Dynamic pricing algorithms using **online learning** for multiple products under inventory constraints.

This repository contains the implementation of online learning algorithms for **dynamic pricing of multiple products under production constraints**, as part of a course project on *Online Learning Applications*.

---

## 🚀 Project Overview

The goal of the project is to design algorithms that dynamically set product prices to maximize revenue while respecting production constraints. Buyers arrive sequentially, each with their own valuation for each product, and purchase any product priced below their valuation.

### Key Features

- Supports **single and multiple products**
- Handles **stochastic** and **non-stationary environments**
- Incorporates **inventory constraints**
- Implements **UCB-based algorithms** and **primal-dual methods** for pricing

---

## ⚙️ Environment Setup

The project is structured around rounds of interaction:

1. The company chooses which products to sell and their prices.
2. A buyer arrives with a valuation for each product.
3. The buyer purchases all products priced below their respective valuations.

### Parameters

- `T` – Number of rounds  
- `N` – Number of product types  
- `P` – Set of possible prices (discrete)  
- `B` – Total production capacity  

---

## 📊 Requirements

The project is divided into five main requirements, building from simple to advanced scenarios:

1. **Single Product, Stochastic Environment**  
   - Build a stochastic environment  
   - Implement **UCB1** algorithm  
   - Extend UCB1 to handle inventory constraints  

2. **Multiple Products, Stochastic Environment**  
   - Build a joint distribution over product valuations  
   - Implement **Combinatorial-UCB** with inventory constraints  

3. **Single Product, Highly Non-Stationary**  
   - Use primal-dual method with inventory constraints  
   - Design best-of-both-worlds algorithm  

4. **Multiple Products, Highly Non-Stationary**  
   - Decompose problem into per-product adversarial regret minimizers  
   - Extend primal-dual method for multiple products  

5. **Multiple Products, Slightly Non-Stationary**  
   - Partition rounds into intervals with fixed valuations per interval  
   - Extend **Combinatorial-UCB with sliding window**  
   - Compare performance against primal-dual method
