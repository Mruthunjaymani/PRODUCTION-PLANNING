# Philbrick Production Planning Optimization

## 📦 Project Summary

This project implements a full production planning optimization model inspired by the classic Philbrick Production Planning problem — often used as a benchmark problem in operations research and supply chain optimization courses.

The model simulates a real-world manufacturing environment with:

- Multiple products
- Multiple plants
- Multiple production processes
- Monthly time periods
- Regional shipping
- Inventory holding
- Capacity constraints
- Demand satisfaction
- Shipping costs

The problem was formulated as a Mixed Integer Linear Programming (MILP) model and solved using **Gurobi Optimizer** in Python.

---

## 🛠 Problem Formulation

The objective is to **maximize total profit**, defined as:

Profit = Revenue - Production Cost - Shipping Cost - Holding Cost

### Decision Variables

- `P_ijkm`: Amount of product `i` produced in plant `j` using process `k` in month `m`.
- `S_ijlm`: Amount of product `i` shipped from plant `j` to region `l` in month `m`.
- `I_ijm`: Inventory of product `i` at plant `j` at end of month `m`.

### Constraints

- Production capacity constraints
- Demand satisfaction constraints
- Inventory balance constraints (multi-period flow balance)
- Inventory storage capacity constraints
- Shipping constraints

---

## 💻 Tools & Technologies


- Gurobi Optimizer
- Gurobi Python API
- Jupyter Notebook (for model development and reporting)

---

## 📊 Solution Outputs

The model generates:

- **Production Plan**  
  Amount of each product produced at each plant, by process and by month.

- **Shipping Plan**  
  Shipment quantities by plant, region, product, and month.

- **Inventory Plan**  
  Inventory levels at each plant for each product by month.

- **Total Maximized Profit**

---

## 🔎 Model Validation

All constraints were verified and satisfied for:

- Production capacities
- Demand fulfillment
- Inventory flows
- Shipping feasibility

The solution is feasible and fully validated.

---

## 🚀 Key Learnings

This project demonstrates the practical application of operations research techniques for solving real-world production scheduling and supply chain optimization problems.

Key areas covered:

- Linear programming modeling
- Multi-product, multi-period planning
- Flow balance constraints
- Capacity planning
- Profit maximization
- Industrial-scale optimization

---

## 📈 Future Extensions

- Incorporating workforce scheduling
- Multi-echelon inventory modeling
- Uncertainty and stochastic demand scenarios
- Supplier constraints for raw material procurement
- Dynamic rolling horizon planning

---

## 🙋‍♂️ Author

> Mruthunjay Mani  
> MS Industrial Engineering 
> Feel free to connect with me on LinkedIn!

---

## 📌 License

This project is for academic and portfolio purposes only. All model formulations are based on publicly available benchmark problems in operations research literature.

