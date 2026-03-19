# Urban Delivery Route Optimization with ZBE Constraints

Optimization project for last-mile delivery planning under operational and regulatory constraints.

This repository contains two Pyomo models:
- **Model 1:** base scenario without ZBE restrictions
- **Model 2:** scenario with ZBE access restrictions and an ECO vehicle investment decision

## Overview

The project models a delivery company operating with a single van that must decide which customers to serve, how to plan the route, and whether investing in an ECO vehicle is economically worthwhile under low-emission zone regulations.

The objective is to maximize profit while considering demand, vehicle capacity, travel costs, time availability, and penalties for undelivered packages.

## Repository structure
```text
.
├── README.md
├── requirements.txt
├── data/
│   ├── customers.csv
│   ├── locations.csv
│   ├── params.csv
│   ├── params2.csv
│   └── zbe_customers.csv
├── notebooks/
│   ├── 01_base_model.ipynb
│   └── 02_zbe_eco_investment_model.ipynb
└── docs/
    └── report.pdf

## Tech stack

- Python
- Pyomo
- Pandas
- Gurobi

## Installation

```bash
git clone https://github.com/bertranvidal/urban-delivery-route-optimization.git
cd urban-delivery-route-optimization
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt




Usage
jupyter notebook

Run the notebooks in this order:

notebooks/01_base_model.ipynb

notebooks/02_zbe_eco_investment_model.ipynb

Report

The full project report is available in docs/report.pdf.

Academic context

This project was developed as part of an academic optimization assignment focused on formulating and solving a realistic MILP problem in urban logistics.